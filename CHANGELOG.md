# Changelog

### **v1.2.0** - Latest

### New Class!
* Introducing the Deprived class! Another member for the B-Company Divison.
    * **Max Health:** `-80%`
    * **Projectile Armor:** `-50%`
    * **Melee Armor** `+80%`
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
> Dev Note: Techman Industries just had an upgrade to one of their arsenal. Somehow, the R&D team were able to bypass the Geneva Convention restrictions and the warranty on the Gauss Rifle. Once it delivers a paylod onto a target, nano globules will eject from a neutralized target. Afterwards, it will seek nearby targets to inflict additional injuries. Potentially saving the industry the added costs of each bullet fired. Techman Industries is not responsible for collateral damage, civilian casualties, or unexpected multi-target liquefaction.

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

#### Recommended mods, but not required:
* `Fridos_Sorted_Boosters` by Fridolin
* `Perfect Boosters` by Localia
* `PingEverything` by Localia
* `BetterMaps` by GTFOModding
* `BetterBioTracker` by GTFOModding
* `Accurate Crosshair` by Dinorush
* `SkipIntro` by Shadsterwolf
* `ChatterReborn` by easternunit100
* `MeleeTimer` by long_walter
* `InLevelCarryOnBack` by Hikaria
> Dev Note: These are recommended, but not needed. Some of these mods with have configs that will be packaged with the mod-pack, but not the mod itself. These aren't necessary, but nice to have on the list.

### v1.1.1
* Fixed a mistake with Shock Trooper's armor not reflecting correctly with the v1.1.0 tweaks.
* Fixed Covert Ops class's melee damage bonus being `45%` when it should be `50%.`
* Fixed a few more typos again!

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

### v1.0.2

* Fixed packaging mistakes which caused files & folders to not unpack the correct way.
* Fixed more typos. Sorry...
* Fixed missing dependency `Junkie Syringe Pack` by ProjectZaero.

### v1.0.1

* Fixed some typos.
* Fixed missing Github links.

### v1.0.0

* Release.