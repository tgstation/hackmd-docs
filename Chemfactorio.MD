---
tags: Design, Chemistry, Factorio
title: Miniaturised Factory chem
---
# Title
[toc]

# Maintainer Design Flows
:::warning
This section describes design flows that are meant to be upheld in the PR process. **PRs that go against this section are subject to closing.** Please do not edit this section unless you are a maintainer. Comments via sidebar are welcomed.
:::

---

## The factory z level
The factory level is an inaccessible Z level that cannot be accessed by human mobs by any means (think like centcomm).

The chemistry player can interact with some mechanism on station, this gives them an advanced camera console like UI, with chem factory components that are buildable, with a view into that Z level, where it has reserved a space for that specific mechanism.

Building a component takes any required costs, and can pull from the global techlathe material silo if neede

### Notes on reservations
These should work like the shuttle transit space reservation, it blocks out an area of useable space, and surrounds it with undestroyable wall turfs. The size of the space reserved is dependent on the mechanism built on the station.

This allows for research of larger mechanisms that give more space.

The user can attach large tanks to the mechanisms, these can be either for input, or output, and create a corresponding input/output node in the appropriate space on the factory z level. There should also be an output for patches/pills

## Gaining chemistry tanks
Chemistry tanks can be ordered from cargo, and contain pre existing bulk precursor chems, empty ones can be built from the science protolathe (chem should have access to this right?)


---
# Non-Maintainer Design Flows
:::info
This section describes various design flows that are not yet incorporated into the maintainer-approved design. **Working towards these flows does not guarantee merge, nor does going against these flows guarantee close. Please resort to `##` and below for heading tags, and preferably `Title (Author)` for easy reference. Titles can be set with YAML metadata. Ping Cobby on Discord if you need assistance embedding/generating your note.**
:::

---

embed notes here

---