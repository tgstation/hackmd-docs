---
tags: Technical, Chat, UI
---
# Runescape-Style Chat

In this document you will find a description of how this system was built, how it functions, and important things to note.

## Chatmessage Datum
At the core of the runescape-style chat ("runechat") is `/datum/chatmessage`, which upon its creation will generate the image apply the animations to display the desired message to the desired client on the desired target.

There are a few things to note about this datum:
- It is client-specific, this is due to the desire for having different languages be interpreted and displayed properly. Different clients will interpret messages in diferent ways, and so the images must be handled on a client-to-client basis.
- Maptext is a fickle beast and must be handled carefully. The majority of texts that are available to BYOND by default are antialiased to a great degree and look VERY blurry. This is why we use the `Small Fonts` font-family.
- Links appear to be automatically wrapped in an anchor element by BYOND, and **must** be escaped/removed before putting the final maptext on the image
- The height of the image is measured using the `MeasureText(...)` proc on `/client` which necessitates having a reference to a client who is on BYOND v513.
- Messages prefaced with a angle bracket (>) will cause the measure proc to fail, resulting in a zero-height measurement. My approach to handling this is by temporarily replacing all html metacharacters to be "m" characters for measuring purposes. [BYOND bug report #2563917](http://www.byond.com/forum/post/2563917).

In an ideal future I would like to only require a single `chatmessage` datum per language variant of a message, and just use the reference to it for handling sending the image to each client. This is difficult to accomplish currently because it would require some sort of central reference or caching system, as when we intercept the message in `Hear(...)` we don't know who else is hearing it.

## Recieving Messages
In similar systems for showing overhead messages, it is often the case that the developers have tied into the point where messages are generated/said by mobs. The runechat system **does not** take that approach; instead, we display messages when they are heard by mobs. This provides the advantage of hearing machines and other sources of messages that otherwise go unnoticed by those who choose to use mob speech procs.

An important thing to note about recieving messages, however, is that when recieving radio messages the speaker is wrapped by a `/atom/movable/virtualspeaker`, which within its `source` property contains the actual `/atom/movable` that spawned the message. This is important as we need the source location to display the message properly to clients.

When a message is recieved, if a client is present on the mob that is hearing it we will create a `chatmessage` datum and it will automatically handle the creation of the image above the speaker. This is done through a call to the `/mob/proc/create_chat_message(...)` proc.