---
tags: Design, Medical, Chemistry, Healing
---
# Medical Design Doc
[toc]
## Maintainer Design Flows
:::warning
This section describes design flows that are meant to be upheld in the PR process. **PRs that go against this section are subject to closing.** Please do not edit this section unless you are a maintainer. Comments via sidebar are welcomed.
:::
### Medical (Department)

Medical is a department where one should be constantly making choices that may not always be optimal, quick but well-thought thinking is key, and there is a sense of accomplishment from overcoming the hurdles that are dynamically presented to you, often by other players who probably have you in their crosshairs as well.

Do note that the department also requires some consideration for the patients. Having to strike a balance between keeping the doctor interested as well as not making it so the patient doesn't ever get to practically play the round again is key.

### Healing Source Categories
I get this question a lot and may refer to items as C# here so the ~~3~~ 4 Categories are below.

1. Healing that is not sourced from the dispenser or plants. Passive healing and white-kit contents are examples of C1.
2. Healing sourced from Chemistry or Plants with a long-term deterrent. Syriniver, Libital, Aiuri are examples of C2.
3. Healing sourced from Chemistry or Plants without a long-term deterrent. Salbutamol, Oxandralone, Atropine are examples of C3.
4. Healing sourced from Surgery. Coronary Bypass, Tend Wounds, Eye Surgery are examples of C4.

> [name=moo] I decided to make a new category dedicated to the longer process of surgery that is hard to conflate with items like sutures/regen meshes.

### Medical Doctor/ Medical (Sub-Department)

#### Overarching Themes

Medical's focus should be on major issues that would require surgery / life-threatening decision making. While they CAN work on more minor ailments, it should be either on downtimes or at a risk of patient overload.

Surgery should be an active process that focuses less on tool-checks and RNG to completing mini-activities (Operation Game? Stardew Valley Fishing?) that would be available to both doctor and patient for faster thoroughput. This would keep both players in the game rather than tabbed out watching the latest runtime video.

### Chemist

#### Overarching Themes
Chemistry should be where doctor's are in need of help: In the grand scheme, this means lower-middle end healing.

Chemistry as in the mechanics will be separated since it extends beyond the job of a Chemist, especially when talking about say Hydroponics/Botanists.

### Reagents/Chemicals
Chemicals that heal should either hardcap at half sustainable damage (not preferred) or provide a longer term ailment that can be relatively non-problematic so long as they aren't 
1) taking the medicine constantly (what we'll call **doping**) 
2) Not requiring long-term exposure, as this would suggest the patient should have been seeking treatment from a doctor instead.

The goal here is to force the patient to decide between "quick-fixes" versus a more proper treatment, which now becomes out of scope for the chemistry realm.

#### Chemical Sources
* Chemical Dispenser/Synthesizers - If it can be made purely through here, it is REQUIRED to fall into [C2](https://hackmd.io/QBwvHy9MTwCShh2gh43RIA?both#Healing-Source-Categories)
* Botany - If the reagent can be made straight from a plant OR a plant can be easily tailored to generate the reagent, it is REQUIRED to fall into [C2](https://hackmd.io/QBwvHy9MTwCShh2gh43RIA?both#Healing-Source-Categories)
* Lavaland - No Restrictions Currently

#### Per-Class Reagents
There should be a maximum of 5 reagents per class, Category Independent ([C2/C3s](https://hackmd.io/QBwvHy9MTwCShh2gh43RIA?both#Healing-Source-Categories)). This helps prevent chem-stacking as well as simply switching over to an equivalent to allow practical doping between meds of similar function.

#### Naming
The purpose of the naming convention is to allow for chem malleability if it requires balance (See: "We can't have this because that's not how it functions in real life!") while also letting people easily know at a glance what the class of the reagent is such as -ibital being your brute healers and -mol being your O2 healing.

New non-element chemicals are REQUIRED (regardless of function) to fall into the following naming convention.

* Root
* Suffix/Prefix pertaining to Class (function) and Damage Type.
* Combination functions such as Omnizine can be considered their own class.

Current Conventions are listed below.

| Class         | Prefix/Suffix  |
| ------------- | ------- |
| Brute Healing | -ibital |
| Burn Healing  | -uri    |
| Oxy Healing   | -mol    |
| Tox Healing   | -iver   |
| Organ Sustain | -rite   |

## Non-Maintainer Design Flows
:::info
This section describes various design flows that are not yet incorporated into the maintainer-approved design. **Working towards these flows does not guarantee merge, nor does going against these flows guarantee close. Please resort to `###` and below for heading tags, preferably `Title (Author)` for easy reference.**
:::

### Medical Machinery (Edge)
Medical should become a primary consumer of power on the station given their machinery assists in keeping other players alive.

To acomplish that goal and to make the medical system more interesting stasis beds should be fragmented into diffrent machines that individually use a lot of electricity. Each machine should be a little bit superior on their own to what stasis beds currently offer, to discourage overuse of formaldehyde.

#### Types:
All of the machines are immobile unless stated otherwise
##### Stabilizers:
Stabilize the organ and provide temporary HP to it as long as you are hooked up to it.

- HEART
- LUNG
- LIVER
##### Life Support:
Prevent you from dying under a fixed amount of hp. Don't prevent you from going into crit, nor do they stop metabolization.
- Basic - 300 HP immobile
- Mobile - 300 HP mobile
- Advanced - 1000 HP immobile

##### Other:
- Dialysis - purges body of chemicals, becomes quicker with better parts.
- Radiation stabilizer - prevents body from taking toxin damage from rads
- Temperature stabilizer - tries to stabilize the body to it's preffered temperature (thinking about lizards and cryot, hercuri etc.)
- Plasmaman stabilizer- a fancy shower that doesnt require the poor guy to be on the floor, but on bed. Prevents plasmaman from burining