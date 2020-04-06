---
tags: Design, Hydroponics
---
# Hydroponics Overarching Goals:
BY ARCANE
* Move away from the meta of speedrunning gaia for plants to grow themselves.
* Prevent rapid speedrunning of hyperpowerful plants that can cure all illnesses and injuries without drawbacks. It should still be possible, but require planning, forsight, and active effort.
* Make the layout of hydroponics meaningful to how the department plays. Redesigning what plants should be placed next to what should be a dynamic process throughout the round.
* Hydroponics trays should benefit more substantially from upgrades, be it from nutrient draw, water capacity, or nutrient capacity.
* Enable combinations of nutrients to get optimal plant stat gains, as some nutrients benefit from quantity, where some provide static stat boosts.

## New Mechanics and how they (are supposed to) work:
### Crosspollination
Adjacent plants with a high enough instability (Anything over 20) will pick a random reagent from the other plant and incorporate that gene into itself. Planting unstable corn next to stable cherries, for example, will cause the corn to gain the sugar reagent from cherries, for example.

However, crossbreeding passively also causes the potency, yield, and instability of 2 adjacent plants to even out over time. If you intend to combine 2 plant's reagents together equally, it's easy enough to do. Moving just one reagent over with no consequences however will take active work to tailor a specific nutrient bath for the donor as opposed to the recipient.

**NOTE ON CROSSPOLLINATION OF CHEMS**
If you have 2 plants next to each other, and you want to prevent them from crossbreeding WITHOUT managing stability, there IS a way to do that, just build single pane glass windows between the trays.

### Plant Grafting
Every plant has at least one type of plant gene that can be grafted off of it. As crosspollination only enables reagents to be moved over, grafting is how you aquire physical traits within the plant, such as Slippery Skin, Bluespace Activity, or Hypodermic Prickles.

To aquire a plant graft, you need to use secateurs in order to cut off a limb of the plant, which costs the plant health, as well as can only be done ONCE per living plant, and only when harvestable. This is to encourage you to actually grow a wider variety of plants to benefit the rest of service.

*Plant grafts should not be invisible. (Sorry).*

### Changes to Reagents
Plant trays all use an actual, internal beaker now in order to determine stat effect. Some of them work based on the amount of the reagent within the tray, where others apply a static effect for every process within the tray.
Most of the general effects of traditional "plant" reagents will be listed below:
##### Quantity Dependant Chems:
* EZ Nutrient: Increases potency and Yield(Slightly), statically increases instability.
* Left4Zed: Increases plant health and stability.
* Robust Harvest: Increases potency (slightly) and yield, decreases instability.
* Ash: Increases health, statically decreases weeds.
* Saltpetre: Increases health, production, and potency.
* Diethylamine: Increases health, yield, but decreases pests and instability.
* Nutriment: Increases plant health.

##### Static Chems
* Ammonia: Increases yield and instability, dynamically increases health slightly.
* Stabilizing Agent: Decreases instability.

##### Weird Special Cases:
* Mutagen: Mutagen deals dynamic toxic damage to the tray, but any time it's inside the tray, it'll roll to attempt to mutate the tray via instability, regardless of quantity.
* Uranium/Radium: As above, but they deal both health and toxin damage to the plant with high quantities within the tray.
* *Several other chems have unique effects as well, as now that it's moved to it's own proc, it's exceptionally easy to add new effects to existing chems, or to make any new chemicals that have different effects on plants.*

### Autogrow
As a replacement to gaia trays, and earthblood being used to make endless god trays, you can now enable autogrow on trays. At the cost of a large portion of power, the tray will drain less nutrients, regenerate a portion of water, and passively decrease weeds and pests. This will enable players to be able to maintain higher mainenance plants, or enable players to spend more time away from their department early in the shift, to make up for the increase in micromanagement required for the new system.
*Other sugestions have included turning autogrow into a kind of stasis mode, which I might want to go in on, but I haven't actually heard much feedback specific to autogrow and it's place within the new system, so this will need some looking at.*

### Experimental Changes
These are subject to change and I am currently workshopping how these will work without making anything too slow, too RNG dependant, or too unlikely to see use in a single round.

*Keep in mind, not every round has to have everything happen within it. Sometime's there's just no miners. Other times, the power goes out in 5 minutes and the station will struggle with it excessively. That's just how it is normally, and a 25 minute shift will happen every once in awhile, even if the overarching design goal is 1 hour long rounds.*

#### Gene Shears
Currently featured in https://github.com/tgstation/tgstation/pull/50387
Enables players to shear off unwanted genes inside a plant, at the cost of health. If you breed your plant to have an exceptionally high endurance, you'll be able to shear off more genes at once, and can get the most benefit from this mechanic overall. Costs 15 plant health every shear, and allows for unique tailoring of plants to match that. However, to make gene shears, you need the experimental tools node. Requires small amounts of iron, uranium, and silver, all of which can now be solidified as a result of chemical solidification reactions through that same PR. I decided on experimental tools over the botanical engineering node, simply because I know it's far, FAR more likely to be researched in the scope of a regular round, and it's been made quite clear that botany players need a way to remove genes for optimal results.

#### Either Higher Nutrient Quantities, or lower nutrient metabilization. 
This is a matter of preference, really. Currently, an un-upgraded, new-style hydroponics tray has 10 units to work with.
This could either be changed to more efficiently use reagents (From 1-0.25 currently), or to contain more reagents. This will need to be determined off of feedback, but as it stands I'm happy with the current values for fully upgraded trays having 50 units, it's just that early resource management that will be a pain.