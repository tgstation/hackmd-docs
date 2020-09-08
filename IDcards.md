---
tags: Design, Access, Cards
title: ID card design
---
# ID card design
[toc]

# Maintainer Design Flows
:::warning
This section describes design flows that are meant to be upheld in the PR process. **PRs that go against this section are subject to closing.** Please do not edit this section unless you are a maintainer. Comments via sidebar are welcomed.
:::

---

## Justification / Outcomes wanted
Right, so right now if a single generous person gets access to the captains card or the spare, everyone and their dog can end up with all access and there's very little way to tell when someone has all access, or their card is modified beyond the default permissions.

I feel that the decision of getting access to large parts of the station should have commensurate increases in how stealthy you appear to the crew. That is, as you gain more and more access, up to and including all access, the type of ID card you have to carry becomes more and more conspicious and roving security, detectives and random busybodies are more likely to spot your elevated access levels.

Furthermore, when getting access to the Access console and selecting roles as an Antag or a greytider or whoever, I feel you should be forced to make tradeoff decisions about what areas you choose to get extra access too, dependent on the type of gear you've managed to acquire.

I want it such that even if the captains spare leaks, or the captain's actual card is also lost to greytide or antags, this does not result in eveyrone having all access, instead, those ID cards are still highly desired for their all access properties.

Finally I want it such that players with all access or lots of access are forced to confront hard decisions about what accesses they can give out to other members of their group and how quickly they can do that.

The outcomes here are that
* People who plan ahead and gather more ID cards are rewarded
* People are forced to make difficult and meaningful decisions about what areas of the station they get access to on their cards
* Granting yourself large amounts of accesses increases the visibility and your risk profile to other staff and security members

The general way in which I hope to acheive this is to make access flag slots and the cards themselves a limited resource with modifiers that lead to player's making strategic decisions.

**Note, some of the limits are literally made up from my brain based on guesswork and subject to change as we thrash out this idea**

## Card levels
Cards are assigned a number of wildcard, and predefined slots based on the Colour of the card and the Trim.

They also have a maximum flag level per wildcard slot that determines the highest level of acces category that specific slot can support.

This means that basic ID cards can only carry a small number of accesses, which means, even with a wallet, you have to make decisions about what accesses you actually grant yourself, or hustle and grind to get yourself access to the higher tier cards, with commensurate increases in your visibility and risk taking.

### Wildcard slots
These slots can have any access assigned to them, up to the maximum allowed by the card type and up to the maximum level allowed to the card.

### Predefined slots
These are slots for specific types of access on the card, they may not be toggled on but the card supports these specific ones if you can turn them on and turning them on does not count towards your wildcard slots.

There are a higher more of these on each card to support departmental accesses, but predefined slots will only grant access to specific types of area.

### Flag levels
Access flags are categorised into levels of access

First the station categories
* Common (Departmental/general/common area accesses)
* Command (Command staff/secure accesses, think bridge/armoury, AI upload etc)
* Private Command (Private head of staff offices, usually only granted to most cards by trimming)
* Captain level (Captains private rooms.)

Now some misc categories
* Centcomm Level (Centcomm area stuff)
* Syndicate level (Syndicate areas off station)

## Types of card
* Grey - The basic card, this has only two wildcard slots, in addition to this, it can only carry common level access flags.
* Silver - The head's card of choice, this has five wildcard slots for extra accesses and can carry up to five common and up to two command level access flags.
* Gold - The card of choice for all access, this can take any/all permission roles it can take Common/Command/Private Command/Captain level flags.
* Centcomm - A gold card that also has centcomm category support.
* Syndicate - A gold card that also has syndicate category support, status item!!
* Deathsquad - Centcomm card but cooler
* Prisoner - No levels of access, predefined prisoner access flags only

#### Disguised chameleon ID 
This will probably be the most controversial aspect of the changes so I've split it out into it's own section as there's a bit to unpack.

* This card can only hold five wildcard slots 
* One at captain level or command/common
* One at command level or common
* The remaining three at common level.

This ties back to the justifications and outcomes presented in the start of the document. Having lots of access should be something that raises your profile, so having a disguised ID should limit the number of slots available so you have to make trade off decisions about amount of access VS stealth level.

It also means you have to decide what accesses you want to target which areas of the station to better achieve your objectives, rather than just the blanket, give myself all areas and not have to confront any hard tactical decisions now or later

### Trims
The "Trim" of the card modifies the predefined slots available - this is so department cards can get the relevant department slots without interfering with wildcard slots

For example, if you have the red security Trim and corresponding software (for the lore nerds), your card will have predefined slots for the security department accesses (security area, brig, break room, prisoner transfer etc).

A silver card with a department trim also gains a pre defined slot to cover that head's private office.

### Trim painter
The head of personnel has a trim painter machine that can repaint a card's trim and reprogram the software, but a card only supports one trim, so a given card can only allow access to one departments flags, and you need to use wildcard slots to access other areas/departments. It's expected this machine can be built by others with a modicum of effort, because note that while it grants the predefined slots, it **does not** toggle them on. So you still need an ID console.


### Concrete examples
A security officer might have a grey card, with security trim, that has the security predefined job flags on, and space for two wild card slots.

If they get access to the ID console, they could choose two more accesses to add to this card, but only common accesses (maybe engineering for example)

The head of security will have a silver card, with the security trim, that has all his accesses and the appropriate command accesses (which take up a wildard slot).

If he gets access to the ID console he can grant himself one extra command level access (maybe he wants AI upload access) and four common accesses, or five common accesses.

The captain has the captains card, it's gold and he can grant any station level accesses to himself. The same for the spare.


## In progress thoughts
Decide if creating new gold cards is something that should be doable and how that might work, at the very least, silver should be obtainable with work, along with your own trim painters so you can get more areas to access if you're willing to put in some time and effort.

---
# Non-Maintainer Design Flows
:::info
This section describes various design flows that are not yet incorporated into the maintainer-approved design. **Working towards these flows does not guarantee merge, nor does going against these flows guarantee close. Please resort to `##` and below for heading tags, and preferably `Title (Author)` for easy reference. Titles can be set with YAML metadata. Ping Cobby on Discord if you need assistance embedding/generating your note.**
:::

---

embed notes here

---