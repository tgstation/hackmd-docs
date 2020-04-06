---
tags: Design, Anomalies, Research
---
# Anomaly cores production

## Justification
We need a new system to control the rare item economy, rare items are very high super tech level items from the techweb, e.g. The Bag of Holding, The Beam Rifle and the Phazon mech.

The problem here is that as soon as you research this item in the Techweb, you can pretty much mass produce them, because they do not require significant amounts of material resource, and the material resources economy is already highly unbalanced.

Fixing that is considered out of scope as it would require changing a very large number of variables.

So although we have control of when the item is introduced (Through techwebs), we can't control how many of the item is produced (or not easily at least) and this leaves us struggling to manage the design and concept of super powerful items as we only have one of the two main variables that it's important to control (when it arrives, and how many of it arrive)

## Design of feature
The plan is to introduce the concept of requiring an Anomaly core to create/build the item (being it's unique powersource or some other lore). The number of Anomaly cores is strictly controlled, which means we can use this to provide a maximum cap on the number of a specific item.

It will also require the Anomaly producers to decide how to best allocate their limited resource. For example, do they want to produce a Phazon or two, or do they want bags of holding and so forth.

To do so we are taking the existing Anomaly cores system and overhauling it, it already touched on some aspects of this with the reactive armours, but didn't go far enough, and lacked the ability to farm the cores in a productive and reliable manner.

## Production of cores
Production of the cores is a two step process, first, raw cores for a specific type of Anomaly core is gathered in the collection phase, then, it is refined into a useable Anomaly core in the Refinement phase via the use of Toxins bombs

### Production of raw cores
The raw cores are ordered via cargo, one core per crate (with a maximum number of raw cores available as per the core limits, this can be LORED as NT only making a certain number of these expensive items available), you start with 2 of **each** type in the science bay, so can produce 2 of each type of core without needing the cargo team to order more.

### Refinement of raw material into useable product
Refining the raw core item into a useable product requires the use of toxins and bomb making. The core must be compressed using an explosion to refine it into something that can be placed into the items.

#### Detonation chamber
A new machine is added, the detonation chamber machine, in which a bomb is placed as well as the raw anomalous matter obtained from the collection process. The bomb would then be "detonated" off-screen and with no damage to the room the detonation chamber is in, to refine the raw material into a core using high heat and pressure.

As the raw matter obtained becomes less and less pure larger and larger bombs are required to refine a useable core.

Small bombs will be required for the first few cores, and then scale up to a Max Cap for the last 2 cores.


## Core limits
There is a maximum limit on the number of each type of anomaly introduced into the round, no more than **8 per type** should be able to exist in a round, this variable should be easily exposed to coders to allow the tweaking up and down per type

### The max limits
Yes the number 8 is pretty much arbitrary, but I wanted to start out with a smaller number on the basis it will be a lot easier to increase this number at a later point, rather than have to turn it **down** with all the associated rage that brings.

In an ideal world the numbers wouldn't be politicised and adjusting them would be a standard thing for maintainers to do, but that is an unlikely event.