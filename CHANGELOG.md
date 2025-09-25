# Changelog

### **v1.4.2** - Latest

### Player Tweaks:
* Added a decimal point for health and infection bar to give a more accurate reading.

### Mod Additions:
- Updated `ExtraToolCustomization` mod to the latest version by this patch's release.
- Added `Skip Intro` mod by Shadsterwolf
- Added `Ping Everything` mod by Localia
- Added `SentryAmmoPercentageScreen` mod by GTFOModding
- Added `Melee Timer` mod by long_walter
> Dev Note: While I believe bug fix and QoL mods should be up to the players to decide what to add in. After multiple playthroughs and tests I got sick and tired of seeing that intro cutscene. The Ping Everything is there to make communications between players easier especially for Bio Tracker user. Sentry Ammo Percentage is to check how much ammo you have left after placing sentries down. Melee Timer is just to give players a better indicator for how long they can hold onto the charge. These are all small mods, so it shouldn't greatly affect gameplay except subtly enhance it.

### Class Tweaks:
* Paramedic:
    * Increased Regen Delay bonus from `-15%` to `-20%`
    * Decreased Initial Ammo penalty from `-25%` to `-20%`
> Dev Note: Changes to regen cap has made the earlier nerf patch a little too harsh for this class.
* Quartermaster:
    * Increased Regen Cap bonus from `+40%` to `+55%`
> Dev Note: Once I figured out how the Regen Cap was being calculated, adjustments were made to the class. With a full Regen Cap booster it is possible to get +100% Regen Cap bonus which will raise the class's regen cap from 30% to 60% max health.
* Courier:
    * Removed Movement Speed bonus of `+10%`
    * Added `Living Bio Tracker` ability. This class will automatically tag all hostile targets within the same room.
> Dev Note: Make the Courier have a more unique identity than a Covert Op 2.0. Now your targets are marked for you, claim your bounty.

### Booster Tweaks:
* Fixed Aggressive Sentry Speed and Damage booster giving the wrong values.
* Increased Muted/Bold/Aggressive `Regen Cap` booster by flat `5%`(total potential value from `30%` to `45%`)
* Changed Bold Regen Cap booster conditional from `Low Health` to `Human Proximity`
> Dev Note: Recently I figured out how regen cap is calculated. Regen cap boosters don't add directly to the base 30%. Instead, they are applied multiplicative. For example, a `+45%` booster raises the cap from `30%` to roughly `43.5%`, not flat `75%`. 
* Increased Muted/Bold/Aggressive `Damage` booster by flat `5%`(total potential value from `30%` to `45%`)
* Increased Muted/Bold/Aggressive `Sentry Damage` booster by flat `5%`(total potential value from `30%` to `45%`)
* Increased Muted/Bold/Aggressive `Explosion Resistance` booster by flat `5%`(total potential value from `30%` to `45%`)
* Increased Muted/Bold/Aggressive `Infection Resistance` booster by flat `5%`(total potential value from `30%` to `45%`)
> Dev Note: Some boosters needed a bit more power as scaling for certain values were not worth taking over the others.

### Enemy Tweaks:
* Scout:
    * Significantly tighten the interval between scout scream and EMP event to prevent killing the scout before the EMP event is triggered.

### Miscellaneous:
* Fixed a large number of README typos.

### v1.4.1

### Class Tweaks:
* Paramedic:
    * Decreased Medipack Efficiency bonus from `+50%` to `+30%`
* Quartermaster:
    * Decreased Supply Pack Efficiency bonus from `+50%` to `+30%`
> Dev Note: I might have overtuned this bonus after more testing and receiving feedback.

### Booster Tweaks:
* Decreased Muted/Bold/Aggressive Medipack Efficiency by flat `5%`
* Decreased Muted/Bold/Aggressive Supply Pack Efficiency by flat `5%`
> Dev Note: Similar to the class tweaks on the same bonuses, this was slightly overtuned. The total potential value with boosters stacked has decreased from `45%` to `30%`.

### Weapon Tweaks:
* Added `MirrorWeapons` mod by Dinorush
> Dev Note: Main and Special weapon slots have been unlocked. There is no longer a restriction to have a Special weapon in a Main slot. For example, you can carry both the Thermal Precision Rifle and Sniper Rifle or both DMRs. This will significantly open up build diversity potential for players to experiment with their chosen class.
* Rearranged all weapons to be easier to scroll through the expanded list. It's in `alphabetical` order based on the weapon's brand not its actual name.
* Disabled the option to equip two of the same weapons in both slots.
> Dev Note: You cannot equip two Van Auken's Sniper Rifle in both slots. Sorry.

### Player Tweaks:
* Decreased AmmoStandardInitial from `350` to `300`
* Decreased AmmoStandardResourcePackMaxCap from `450` to `400`
* Increased AmmoSpecialInitial from `250` to `300`
* Increased AmmoSpecialMaxCap from `450` to `550`
* Increased AmmoSpecialResourcePackMaxCap from `350` to `400`
> Dev Note: Lots of new potential options thanks to the MirrorWeapons mod. To prevent some balancing issues, I will have to readjust a lot of the weapons to be more unified in its initial ammo, max ammo capacity, and resupply efficiency numbers. As a result, Special weapons will get an ammo buff while Main weapons will get the opposite. This would mean that Ammo Supply Efficiency will be more important than before, so try out Quartermaster and the appropriate boosters.

### Ammo Tweaks:
* All former special weapon's bullet cost has been increased between `0.1 - 5.0` based on respective weapons. 
> Dev Note: This was done to counteract the new increased unified maximum ammo capacity.

---

### v1.4.0

### Weapon Tweaks:
* Updated `ExtraWeaponCustomization` mod to v3.7.10
* Changed name of `Bio-IR-Dot Tracker` to `Advanced Thermal Tracker`
* Changed name of `Bataldo Single Slug` to `Bataldo Single Slugger`
* Changed name of `Buckland Reserve Hemorrhage Shotty` to `Buckland Hemorrhage Shotgun`
* Changed name of `Mastaba Explosive Shrapnel Cannon` to `Mastaba Explosive Cannon`
* Changed name of `Mastaba Explosive Shrapnel Rifle` to `Mastaba Explosive Rifle`
* Changed name of `Buckland Hemorrhage Shotgun` to `Buckland HEL Shotgun`
* Changed name of `Techman Hemostasis Medic SMG` to `Techman Hemostasis Medic Gun`
* Changed name of `Van Auken W-Pen Sniper Rifle` to `Van Auken Sniper Rifle`
* Changed name of `Techman Nano-Payload Gauss Rifle` to `Techman Nano Gauss Rifle`
* Renamed all weapons' bottom text to include what weapon type it is to prevent confusion with class specialization bonuses.
    * For example: Thermal Precision Rifle(Sniper) or Heavy Assault Rifle(Rifle)
> Dev Note: Changed names to be less of a mouthful to say. And the subtext should be players a better idea on their classes.

* Added `BetterBioTracker` mod by GTFOModding.
* Bio Tracker now has two modes: Thermal or Tracker mode.
* ADS has been changed to old ADS(Pre-R6).
* Decreased target sizes on radar by `20%`
> Dev Note: Bio Tracker should feel more impactful than just a scan tool. Thermal should allow to see in the dark, but lose tracker mode. So knowing when to switch between mode is important. You can still tag enemies in both modes. Also the old ADS was simply more cinematic than the current vanilla version.

### Booster Tweaks:
* Fixed a mistake with an Aggressive Main Damage booster giving a negative Main Damage effect instead of a negative Special Damage effect.
> Dev Note: I believe the booster system is in a somewhat decent spot in terms of balance. It should be giving players a boost to their class or playstyle.

### Class Addition, Changes, & Bug Fixes:
* Updated `GTFuckingXP` mod to v2.4.9
* Introducing the Courier class! Another member for the B-Company Divison.
    * **Heavy Revolver:** `+50%`
    * **Sniper:** `+50%`
    * **Shotgun:** `+50%`
    * **Tripmine:** `+50%`
    * **Movement Speed:** `+10%`
    * **Starting Ammo/Tool:** `+20%`
    * **Ammo Cost Efficiency(Tool/Gun):** `-20%`
    * **Infection Resistance:** `-70%`
    * **Explosion Resistance:** `-70%`
    * **Bullet Resistance:** `-70%`
    * **Bleed Resistance:** `-70%`
> Dev Note: While this class is the fifth in the division, technically it's the B-Company's fourth class. Prisoner doesn't really count towards the class count for each division as it is just the vanilla experience. Plus I was trying really hard to find a home for the heavy revolver as it doesn't have one in any of the other classes. Heartaches by the numbers.

* Re-organized all of the class's specialized weapon bonus to proper reflect their damage bonus effects.
    * For example: Covert Op's Precision Rifle bonus was affecting assault rifles too. 
> Dev Note: The class system utilitzes the vanilla game's booster system to affect weapons within a specific category. Unfortunately this can cause some weapon bonuses to overlap with other classes. The perfect example of this issue is the difference between a HEL shotgun and a regular shotgun. They are both shotguns but one is HEL which uses HEL weapon buffs instead of the shotgun ones.

* Marine:
    * Removed `DMR` Specialization
        * Includes: Hanaway DMR & Hanaway Double-Tap
    * Fixed Bullpup Rifles Specialization not working as intended

* EOD Specialist: Renamed to `Demolitionist`
    * Name was changed to sound more better and clearer.

* Tool Specialist: Renamed to `Specialist`
    * Name was altered since EOD Specialist name was changed.

* Covert Ops: Renamed to `Covert Op`
    * Increased Sniper/Precision Rifle & Melee Damage bonus from `50%` to `60%`
    * Increased Max Health penalty from `-20%` to `-30%`
    * Removed accidental usage of `Assault Rifle` specialization(within code)
    * Added `DMR` Specialization
        * Includes: Hanaway DMR & Hanaway Double-Tap

* Field Technician:
    * Added Ammo Cost Efficiency debuff of `-10%`
    * Increased Hacking Skill bonus from `55%` to `60%`
    * Increased Sentry CPU bonus from `30%` to `40%`
    * Increased Sentry Damage from `30%` to `50%`
    * Removed accidental usage of Sentry `Long-range` and `Short-range` damage bonus of `30%`.
    * Fixed a potential issue with -40% damage reduction penalty affecting the sentry turrets.
> Dev Note: There was an accidental addition of Long-range and Short-range damage bonus that make significant boost to sentry power that was unintended. But to prevent a potential massive nerf to their damage, I am increasing the overall base damage bonus of sentries.

* Prisoner:
    * Added a warning for difficulty.
> Dev Note: Every other changes are still in effect, even though class system isn't being used with Prisoner. So I might as give a small warning.

* Abhuman:
    * Increased Max Health bonus from `100%` to `150%`
    * Decreased Movement Speed penalty from `-40%` to `-30%`
    * Fixed incorrect bonus values on the class for melee damage, range, and hitbox.
> Dev Note: Althought this is a meme class, the negative effects are still higher than its positive counterpart. Also the class had incorrect values in its class description.

### Miscellaneous:
* Improved the README.md to provide a link to a list of recommend mods within Thunderstore's wiki. Link [Here!](https://thunderstore.io/c/gtfo/p/Carb_Crusaders/GTFriendlyO/wiki/4030-recommend-mods/)

### v1.3.1

### General Tweaks:
* Fixed a mistake on installing the wrong version of ExtraWeaponCustomization mod.
> Dev Note: Accidentally used the wrong version number 3.7.7 instead of 3.7.9 by the time of this patch comes out.

### Enemy Tweaks:
* Fixed typo regarding Shadow enemies having cloak abilities.
> Dev Note: Cloaking was originally planned but it was buggy with Shadow enemies in particular. Instead Shadow enemies will create fog spheres when killed, Fog Repellants and Fog Turbines are a great counter.

* Increased Scout's max tentacle range from `30.0m` to `60.0m`
* Increased Scout's tentacle speed from `7.5m` to `10.0m`
* Changed Scout's tentacle colors from `black` to `cyan`
* Added Sound IDs to the EMP Ability.
* Shorten the activation transition between `Shout` and `EMP` abilities.
> Dev Note: Increased the Scout's tentacles to be more overall riskier to kill. Good positioning, long-range weapons, and/or using cover with melee will be your best options. The cyan tentacles will be more consistent with this EMP colored scream as well as bring better visibility to them. With the added sound effect, it should be much easier to tell when the EMP event is starting.

* Shadow enemies will spawn fog spheres upon death.
    * Fog Distance(expands) from minimum `3.0m` to maximum `6.0m`
    * Fog Activation delay of `0.1s`
    * Audio sound cue when fog appears.
    * Fog will inflect infection with a rate of `0.05%` per second.
    * Fog Duration of `30s`
> Dev Note: Fog repellant and turbines are your best friend against this area-of-effect denial ability. Or kill them before they get too close to the team. Either way a Tool Specialist is a strong counter to this as long as they have the right consumable(Fog Repellant)

### Weapon Tweaks:
* Increased Tracker Precision Rifle Damage from `26.9` to `28.1`
* Increased Tracker Precision Rifle Hipfire Spread from `3.0x` to `2.5x`

### Syringe Tweaks:
* Increased Damage from Virus Bomb Syringe from `250` to `300`
* Increased Damage from Virus Nuke Syringe from `500` to `600`
* Decreased Range of Virus Nuke Syringe from `10.0m` to `7.5m`
> Dev Note: Kaboom? Yes Dauda, kaboom.

---

### v1.3.0

- Important note regarding boosters in the Booster Rework section. I highly reccomend you read it, thank you.

### Weapon Tweaks:
* Updated `ExtraWeaponCustomization` mod to v3.7.9
* Replaced muzzle flash effect from all guns to pistol muzzle flashes.
> Dev Note: For some reason this game's muzzle flash feels significantly more offensive to the eyes than any other FPS game. The flashing lights were already removed, but some guns had egregious muzzle effects. Now, it's possible to use Reserve/Full-Auto guns for longer periods of time. Unfortunately, this does make the guns feel a little less realistic. Yet, I would trade that for less eye strain in a heartbeat.

### Enemy Tweaks:
* Changed Flyer's `Bleed` projectiles to `Explosive` projectiles.
    * Explosive Damage of `5%`
    * Radius of `2.5m` to `5.0m`
    * Can alert nearby enemies within explosion radius of `5.0m` to `10.0m`
* Added Large Needler to the `Bleed` ability list.
* Increased Child's minimum explosion damage from `1.5m` to `2.0m`
* Improvements to Shadow variants.
    * Fixed a mistake with Shadow enemies having the wrong amount of Tag time. It should be `10.0s` now, instead of `30.0s`
    * Increased Shadow's health from `34.0` to `40.0`
    * Shadow enemies can no longer be pushed or be damaged with backstab multiplier bonus.
    * Increased Shadow enemies global speed from `80%` to `85%`(They will move/attack a bit faster)
> Dev Note: Flyers should have a bit more identity as well as incentivize explosive resistant more. Shadow enemies felt like they need a bit more attention. The Large Needler inclusion will also add more value to Bleed Resistance for the Marine class.

### Class Balance:
* Fixed class balance tweaks from v1.2.1 not reflecting properly.
* Added `WorseHackingMiniGame` by Cactus.
    * Disabled mod's increased hacking patterns and size. Vanilla hacking pattern.
    * Enabled moving solution area. The solution bar will now steadily move while trying to solve.
* All Classes(except Field Technician, EOD Specialist, HEL Diver, and Abhuman) baseline Hacking Proficiency is slightly decreased by 20%.
    * To give you more perspective: the final third hacking pattern is now `2` solution bar instead of the default `3` bars. Field Technician's baseline is `5` bars, HEL Divers's baseline is `6` bars.
* Adjusted Field Technician, EOD Specialist, HEL Diver, and Abhuman's Hacking Proficiency text(not values) to reflect the new lowered baseline value. Their values are untouched, only their text description.
> Dev Note: This baseline decrease will not show up in their class descriptions, the adjusted values will go to the classes that have the biggest changes. The main reason for this change is to promote the Field Technician class to utilize their hacking skills as well as lock melters to have more value. Otherwise in worse case scenario, you will have to decide to either destroy the door or ignore a loot container. 

* **Paramedic**
    * Added `Med Efficiency` properties
        * Gains Healing Pack Efficiency bonus of `+50%`
    * Decreased Health Regen Delay from `-40%` to `-15%`
    * Increased Revive Health from `+60%` to `70%`
    * Slight improvements to class description.
> Dev Note: Give Paradmedics more incentive to hold and use Medipacks; fulfilling their roles more. Also the Revive Health change is to increase the health given to be slightly above 50%.

* **Quartermaster**
    * Added `Supply Efficiency` properties
        * Gains Ammo Pack Efficiency bonus of `+50%`
    * Decreased Initial Ammo bonus from `+50%` to `+20%`
    * Slight improvements to class description. Changed plurals to singulars for HMG/LMG/MP for better clarity.
> Dev Note: Give Quartermaster more incentive to hold and use Ammo and Tool Resupply Packs.

* **Abhuman**
    * Increased Melee Damage bonus from `50%` to `75%`

### Syringe Rework:
* **I2-LP Heal Syringe**
    * Removed Health Regen properties
    * Decreased Health Recovery from `24%` to `10% - 20%` (Vanilla: 5% - 15%)
> Dev Note: Vanilla GTFO gave 3% to 10% infection when used, which was removed. It's not a replacement for medipacks, but a decent subsitute.

* **IIx Melee Syringe**
    * Removed Healing properties
    * Replaced with Movement Speed buff of `10%` for `300s(5min)`
    * Decreased Melee Buff Timer from `999s(16.65min)` to `300s(5min)` (Vanilla: 8.0s)
    * Reintroduced Infection from `0%` to `0% - 10%` (Vanilla: 3% - 10%)
> Dev Note: Keep in mind that Melee Buff's baseline damage multiple is 3.0x. So a sledgehammer's heavy damage of 39.5 will do a total of 118.5 with the syringe(not counting boosters). The Van Auken's Sniper Rifle does a baseline damage of 125.5.

* **Speed Syringe**
    * Removed Health Regen properties
    * Increased Movement Speed buff from `14%` to `40%`
    * Decreased Movement Speed duration from `90s(1min30s)` to `60s(1min)`
    * Increased Infection from `5%` to `5% - 10%`

* **Adrenline Syringe**
    * Increased Movement Speed buff from `10%` to `15%`
    * Increased Movement Speed duration from `90s(1min30s)` to `120s(2min)`
    * Increased Infection from `5%` to `5% to 15%`
    * Increased Health Regen duration from `8s` to `10s`
    * Increased Health Regen per tick from `0.4` to `0.5`

* **IV-LP Syringe** Renamed to `Heal Munitions Drain Syringe`
    * Added Main/Special/Tool Ammo properties
        * Sacrifices `20%` of Main/Special/Tool ammo
    * Added Health Regen properties
        * Gain Health Regen of `1%` per second for a duration of `200s`
    * Added Disinfection properties
        * Applies Disinfection of `30%`

* **Virus Syringe** Renamed to `Virus Bomb Syringe`
    * Reworked all properties
    * Increased Infection from `10%` to `15%`
    * Added Self-Destruct properties
        * Explosion damage of `250` over an area of `5.0m`
        * Delay Explosion damage by `10s`
    * Added Damage-Over-Time properties
        * Applies DoT damage of `15.0` after delay
        * Delay DoT damage by `10s`
    > Dev Note: Try not to stick close to your teammates with this one.

* **Antibiotic Syringe**
    * Decreased Disinfection from `40%` to `30%`

* **Surge Syringe**
    * Removed Movement Speed properties
    * Removed Infection properties
    * Added Healing properties
        * Applies Healing of `100%`
    * Added Damage-Over-Time effect properties
        * Applies DoT damage of total `60%` over a duration of `300s`
        * Delay DoT damage before applying of `30s`

* **Recovery Syringe**
    * Increased Health Regen total of `20` to `30`
    * Increased Duration to `180s(3min)`
    * Added Movement Speed properties
        * Applies Movement Speed decreases by `10%` over `3min`

* **Rage Syringe**
    * Reworked all properties
    * Added Melee Buff Timer properties
        * Applies 3x Melee Damage over a duration of `600s`
    * Added Healing properties
        * Applies Healing of `50%`
    * Added Health Regen properties
        * Applies Health Regen of total `50%` over a duration of `100s`
    * Added Movement Speed properties
        * Applies Movement Speed buff of `10%` over a duration of `600s`
    * Added Infection properties
        * Applies Infection of `25%`
    * Added Damage-Over-Time effect properties
        * Applies DoT Damage of `50%` over a duration of `1s`
        * Delay DoT damage after `600s`

* **Antibiotic-XV-LP Syringe** Renamed to `Ammo Symbiotic Regurgitant Syringe`
    * Added Main/Special/Tool Ammo properties
        * Gain `35%` of Main/Special/Tool ammo 
    * Added Damage-Over-Time properties
        * Applies DoT damage of total `70%` over a duration of `70s`
        * Delay DoT damage before applying of `10s`
    * Added Infection properties
        * Applies Infection of `30%`

* **Hallowed Virus Syringe** Renamed to `Virus Nuke Syringe`
    * Reworked all properties
    * Increased Infection from `20%` to `25%`
    * Added Self-Destruct properties
        * Explosion damage of `500` over an area of `10.0m`
        * Delay Explosion damage by `10s`
    * Added Damage-Over-Time properties
        * Applies DoT damage of `25.0` within `1s` after delay
        * Delay DoT damage by `10s`
    > Dev Note: Yes, you will die.

* **Recovery Syringe II**
    * Increased Health Regen total of `35` to `50`
    * Increased Duration to `180s(3min)`
    * Added Movement Speed properties
        * Applies Movement Speed decreases by `-15%` over `3min`

* **Antibiotic-IX-REC Syringe**
    * Decreased Disinfection from `40%` to `30%`
    * Increased Healing from `15%` to `25%`
    * Added Health Regen properties
        * Gain Health Regen of `2.0` per second over a duration of `10s`

>Dev Note: A lot of these tweak, rework, and balance changes are meant to make syringes have a bit more variety to them. While some of them will become niche, at least they have more interesting application based on circumstances.

### Booster Rework:
* Added `Custom_Boosters` mod by Endskill
* All boosters will have 99 charges left, and will no longer be consumed.
    * **IMPORTANT NOTE:** Please be advised that any boosters you currently own will be removed to accommodate the new custom boosters. You will be given 20 Muted, Bold, and Aggressive boosters to play around with.
* Removed artifact pickups in-game.
* Removed most mentions of artifact/booster module pickups on UIs, HUDS, and menus.
> Dev Note: Disabling artifact pickups can potentially change item distribution in containers or level layout. I will observe closely for any potential issues. Please send an issue ticket in the Github, if any problems arise.

* **General**
    * Significantly decreased **Muted** Booster's bonuses which carries no negative penalties
    * All **Bold** Boosters will carry a moderate penalty to match with equal bonus
    * All **Aggressive** Boosters will carry a more significant penalty to match with a higher bonus
    * All Boosters will carry their maximum penalty and bonus numbers. No more RNG on minimum/maximum stats.
> Dev Note: A lot of boosters have mainly moved to the class system, so their power boost is not longer required. As a result this system will be nerfed heavily to keep it "balanced" between the two systems.

* **Muted**
    * Separated all Muted boosters with two effects for some, not all.
    * Muted Boosters will carry very weak positive effects, while carry zero negative effects.

* **Bold**
    * Separated all Bold boosters with two or more effects. All Bold boosters will only carry one effect with a single condition at a time.

* **Aggressive**
    * Separated all Aggressive boosters with two or more effects. All Aggressive boosters will only carry one effect with a heavy negative effect.

> Dev Note: These changes were made to prevent easily overstacking attributes with boosters and classes. Most of the original booster system were regulated to the class sytem. While it's still possible to stack on a particular attribute, the required effort is higher. This will incentize players to theorize which combination works best for yourself and the team.

#### Miscellaneous:
* Fixed README to reflect some of the newer changes.
* Added recommended mods in the README.
    * Removed recommend mods list from the CHANGELOG.

---

### v1.2.1

### Class Tweaks:
* Decreased Marine's Starting Ammo bonus from `+25%` to `+20%`
> Dev Note: The Marine is already a solid class. With the added Bleed Resistance on top of the buffed starting ammo makes them slightly too efficient at their job.
* Decreased Deprived's Melee Armor from `+80%` to `+60%`
> Dev Note: I might have went a bit overboard with the Deprived class.Since a single booster can make them immune to all melee damage. It should at least require up to 2 boosters to do so. Booster rework is coming in v1.3.0 to help balance out this system.

### Weapon Tweaks:
* Removed Reload Time(0.0s) on Reserve Weapons to prevent confusion. (Cannot change Clip Size to 0, since that messes with Ammo)
* DoT damage should no longer work on Locks.    

* **Triple Barrel**
    * Added "Holding Trigger fires continuously" trait while Hipfiring.
    * Added "Fire all three shots at once" trait while Aiming.
> Dev Note: Using this ability with 1 or 2 bullets remaining in the chamber will subtract from the reserve.
* **5-B Bullpup**
    * Increased Max Ammo Capacity from `416` to `442`
* **3-B Carbine**
    * Increased Damage from `3.2` to `3.3`
* **Gauss Rifle**
    * Increased Bullet Damage from `30.3` to `40.3`
    * Increased Precision Multiplier from `1.1x` to `1.5x`
    * Decreased Explosion Damage from `20.0` to `10.0`
* **AR-30**
    * Decreased Damage from `7.1` to `7.0`
    * Increased Clip Size from `25` to `30`
    * Decreased Max Ammo Capacity from `282` to `255`
    * Decreased Reload Time from `2.0s` to `1.8s`
    * Decreased Hipfire Spread from `2.375x` to `2.0x`
* **Heavy SMG**
    * Decreased Max Ammo Capacity from `417` to `391`
* **DMR**
    * Decreased Max Ammo Capacity from `192` to `187`
    * Decreased Magazine Size from `15` to `10`
    * Decreased Hipfire Spread from `2.5x` to `0.5x`
    * Increased Pierce Limit from `0` to `1`
    * Increased Precision Multiplier from `0.87x` to `0.97x`
    * Increased Shot Delay from `0.25s` to `0.3s`
* **Double-Tap**
    * Increased Precision Multiplier from `0.9x` to `0.95x`
    * Decreased Reload Time from `2.15s` to `2.0s`
    * Decreased Hipfire Spread from `3.5x` to `2.5x`
* **MP2**
    * Increased Max Ammo Capacity from `661` to `737`
    * Decreased Hip Spread by `0.1x`
* **MP1**
    * Decreased Pierce Limit from `2` to `1`
    * Decreased Stagger Multiplier from `5.0x` to `2.0x`
    * Increased Hip Spread by `0.1x`
* **Reserve HMG**
    * Increased Max Ammo Capacity from `662` to `742`
* **Explosive Burst Rifle**
    * Decreased Pierce Limit from `3` to `0`
    * Increased Stagger Multiplier from `1.0x` to `1.2x`
* **Hemorrhage Shotgun**
    * Decreased Ammo Capacity from `147` to `110`
* **Hemorrhage Reserve Shogun**
    * Added Charge-up of `0.2s`
* **Choke Shotgun**
    * Increased Damage from `6.2` to `6.4`
* **Revolver**
    * Increased Precision Damage Multiplier from `0.74x` to `0.87x`
    * Increased Stagger Multiplier from `1.0x` to `1.1x`
* **Pump-Action Shotgun**
    * Increased Damage from `5.0` to `5.4`
* **Choke Mod Shotgun**
    * Increased Damage from `5.9` to `6.2`
> Dev Note: I decided to another balance pass on many of the weapons. A lot of them need some tweaking to reflect their new identity within the pack. Very strong weapons that can kill everthing with ease should have a bit of downside with their max ammo. Of course I am still keeping an eye on balance regularly. Feedback is very important, so please let me know on MTFO Discord or Github Repo.

#### Miscellaneous:
* Fixed typos. Phew, crisis averted!
* Added some wiki pages! Check them out in the Thunderstore!

---

### v1.2.0

### New Class!
* Introducing the Deprived class! Another member for the B-Company Divison.
    * **Max Health:** `-80%`
    * **Projectile Armor:** `-50%`
    * **Melee Armor:** `+80%`
    * **Movement Speed:** `+30%`
    * **Range Damage:** `+50%`
    * **Melee Damage:** `+50%`
    * **Initial Ammo(Tool/Gun):** `-50%`
    * **Infection Resistance:** `95%`
    * **Explosion Resistance:** `95%`
    * **Bullet Resistance:** `95%`
    * **Bleed Resistance:** `95%`
    * **Bioscan Speed:** `+50%`
    * **Terminal CPU Speed:** `+50%`
    * **Double Jump** 
> Dev Note: Another joke class to even out the system with 4-4-4 for each division. The Deprived is truly a class where you do so much damage, but aren't allowed to take a hit. Is it stupid? Yes. That's why it belongs in B-Company!!

#### Class Tweaks:
* Increased the Marine's initial Ranged Ammo from `+15% to +25%`
* Added `Bleed Resistance` bonus to the Marine: `+50%` Res.
* Added `Bioscan Spd.` buff to the HEL Diver: `25%` Spd.
* Added `Infection Res.` buff to the Abhuman: `50%` Res.
* Changed wording of some classes which said `Gun Ammo` to `Ranged Ammo`.
* Changed wording of `Computer CPU Speed` to `Terminal Speed`.
* Fixed wording on some of the classes' description.
> Dev Note: Mainly buffs to certain classes. Mainly the Marine class, make them a bit more enticing to use since the other classes fill a niche. Marine should be able to handle other range enemies a bit better.

#### Weapon Tweaks:
* Updated ExtraWeaponCustomization to `v3.7.7`
* All projectiles will show graphics when hitting terrain (bullet holes, dust, and sound).
* Upgraded the `HEL Revolver` and `Heavy Revolver`
    * Removed HEL Revolver piercing capability(never meant to have any).
    * Revolver bullets will "ricochet" off walls that has a chance of hitting an enemy target(Experimental).
* Changed the name of `Santonian Sledge` to `Santonian Slugger`
* Changed the name of `Bataldo Knife` to `Bataldo Hunter's Edge`
* Changed the name of `Omneco Drillhead` to `Omneco GPR Drillhead`
* Changed the name of `Rickman Grabthar` to `Mak'Tar Grabthar`
* Changed Gauss Rifle's full name from `Techman Shrapnel Gauss Rifle` to `Techman Nano-Payload Gauss Rifle`
* Upgraded the `Gauss Rifle's` projectile to have homing properties.
    * **Projectile count:** `20`
    * **Projectile Damage:** `2.0`
    * **Projectile Speed:** `7.5`
    * **Initial Homing Strength:** `2.0 for 1.0s`
    * **Base Homing Strength:** `5.0`
    * **Projectile Lifetime:** `15.0s`
    * **Homing Delay:** `0.2s`
    * **Target Mode:** `Normal`
    * **Target Priority:** `Distance`
    * **SearchStopMode:** `None`
> Dev Note: Techman Industries just had an upgrade to one of their arsenal. Somehow, the R&D team were able to bypass the Geneva Convention restrictions and the warranty on the Gauss Rifle. Once it delivers a payload onto a target, nano globules will eject from a neutralized target. Afterwards, it will seek nearby targets to inflict additional injuries. Potentially saving the industry the added costs of each bullet fired. Techman Industries is not responsible for collateral damage, civilian casualties, or unexpected multi-target liquefaction.

### New Mods!
* `LightsAdjustment` by Untilted
* `Trajectory_Lines_When_Placing` by Localia
* `SentryGunEverywhere` by Localia
* `PacksHelper` by Localia
* `Parry` by CellSkippers
* `FasterHackingMinigame` by Untilted
* `PreciseUI` by Andocas
* `ResourceStack` by Hikaria
* `GTFO_ShootInTheAir` by Fody55
* `WeaponStatShower` by DacreDOLOLO
    * Parrying does not reward health or ammo. However, you can parry enemy projectiles back which deals 18.1 Damage w/2.0x Precision Multiplier. For reference, a regular Needler(Shooter)'s health is roughly between 30.0-40.0. You can also parry your teammates bullets w/2.0x Damage Modifier. Why? Because why not. Try parrying your Covert Ops's Sniper Rifle. Good luck!
> Dev Note: All of these mods were intended with this pack to help even out the class dynamics. SentryGunEverywhere will help FieldTechnicians. LightsAdjustment will make flashlights, glowsticks, and etc feel more impactful. Parry will allow melee users have more ways to tank hits for the team. ResourceStack will allow for consumable pickups for Paramedic and Quartermaster. And the rest of the mods are very helpful!

#### Enemy Tweak:
* Decreased Stalker(Snatcher)'s damage per second from `4% to 3%`. Total damage from `40% to 30%` over 10.0s.
> Dev Note: With the new change to the player's base regen cap, the snatcher's damage should reflect that. The design philsophy has always been to punish and kill players who only rely on their baseline regen cap. Having them do 10% more than regen cap doesn't seem fair anymore.

#### Tool Tweaks:
* Increased Friendly Fire damage modifier for all four sentry types by flat `10%`
* Re-organized many of the Damage Booster Effects to properly assigned classes.

#### Miscellaneous:
* Added config files into the package to further tweak the experience.
* New Thunderstore wiki-pages for some of the main features.
* Fixed a few more typos. My favorite part!

---

### v1.1.1
* Fixed a mistake with Shock Trooper's armor not reflecting correctly with the v1.1.0 tweaks.
* Fixed Covert Ops class's melee damage bonus being `45%` when it should be `50%.`
* Fixed a few more typos again!

---

### v1.1.0

#### Player Tweaks:
* Decreased Player's base regen cap from `40% to 30%`
* Decreased Player's regen per second from `2.0 to 1.0`
* Decreased Player's sprinting speed from `65% to 60%`
* Decreased Player's walk step length from `2.5m to 2.0m`
* Decreased Player's sprint step length from `3.0m to 2.2m`
> Dev Note: I have noticed that some players were able to get away with a lot of situations simply because their regen cap and speed was forgiving enough when stacked with other regen-based boosters. Please keep in mind that these numbers are still higher than vanilla, it's just not as overtuned anymore.

#### Class Tweaks:
* Decreased **Shock Trooper's** Melee & Projectile Armor from `40% to 30%`
* Increased **Shock Trooper's** Movement Spd penalty from `-20% to -25%`
> Dev Note: While I am not a fan of simply nerfing without compensating, but there are few instances where I don't have a lot of options. Shock Trooper is just too good when stacking multiple bonuses.

#### Weapon Tweaks:
* Decreased maximum ammo capacity for **Explosive Shrapnel Rifle** from `103 to 80`
* Decreased reload time for **Explosive Shrapnel Rifle** from `4.2s to 3.8s`
* Decreased maximum ammo capacity for **Explosive Shrapnel Cannon** from `65 to 50`
* Decreased reload time for **Explosive Shrapnel Cannon** from `4.5s to 4.0s`
* Decreased maximum ammo capacity for **Explosive Shotgun** from `49 to 30`
* Decreased bullet damage of **Explosive Shotgun** from `1.0 to 0.5`
* Decreased bullet damage of **Triple Barrel Shotgun** from `5.5 to 5.0`
* Decreased maximum ammo capacity for **W-pen Sniper Rifle** from `24 to 20`
* Decreased reload time for **W-pen Sniper Rifle** from `5.0s to 4.3s`
* Decreased maximum ammo capacity for **Gauss Rifle** from `48 to 40`
* Increased maximum ammo capacity for **Tracker Precision Rifle** from `91 to 98`
* Increased maximum ammo capacity for **Choke Mod Shotgun** from `49 to 54`
* Increased maximum ammo capacity for **Pump Action Shotgun** from `55 to 58`

> Dev Note: Some weapons were overperforming because their max ammo cap was a bit too high. In some rundowns where ammo was plenty, this allowed some weapons to outshine other guns in almost every situation. Unfortunately, this led to other players feeling less impactful within the team.

#### Tool Tweaks:
* Increased detection range of **Burst Sentry** from `25.0m to 40.0m`
* Decreased detection angle of **Shotgun Sentry** from `70.0 to 60.0`
* Increased detection range of **Shotgun Sentry** from `10.0m to 15.0m`
* Increased detection angle of **Auto Sentry** from `50.0 to 60.0`
* Increased detection range of **Burst Sentry** from `25.0m to 40.0m`
* Added **Burst Sentry** ability to do backstab damage.
> Dev Note: Fixed a few awkward attributes regarding the Sentries.

#### Melee Tweaks:
* Decreased range of Melee **Sledgehammers** from `3.0m to 2.3m`
* Decreased range of Melee **Knives** from `2.0m to 1.9m`
* Decreased range of Melee **Spears** from `4.0m to 3.5m`
* Decreased range of Melee **Bats** from `2.25m to 2.0m`
* Decreased base stamina cost of **Sledgehammer** in combat from `0.4 to 0.35`
* Decreased base stamina cost of **Sledgehammer** out of combat from `0.4 to 0.3`
> Dev Note: The new melee ranges might have been overtuned which made the visual feedback between the perspective and actual damage awkward. It is still overall higher than vanilla range, but as much as before.

#### Enemy Tweaks:
* Decreased knockback velocity of **Tank's** tentacle attacks from `12.0 to 10.0`
* Increased bleed damage interval from `0.5s to 1.0s.` (total damage went from `10%` to `5%` over the duration) 
> Dev Note: Tweaked two abilities down to allow for players a bit more avenue for counterplay.

#### Miscellaneous:
* Fixed a little bit more typos here and there.
> Dev Note: Final note regarding the overall vibe of this balance patch. While it's an overall nerf to the many things, keep in mind that this will incentize teams to emphasizing on their strengths while compensating for each other's weaknesses. The pack's goal is to make the experience more accessible, but don't remove all of the difficulty and challenge of the base game.

---

### v1.0.2

* Fixed packaging mistakes which caused files & folders to not unpack the correct way.
* Fixed more typos. Sorry...
* Fixed missing dependency `Junkie Syringe Pack` by ProjectZaero.

---

### v1.0.1

* Fixed some typos.
* Fixed missing Github links.

---

### v1.0.0

* Release.