# Changelog

## **v2.3.0** - Latest

* **Personal Note:** It's generally okay to update any mods whenever they are available. Regular bug fixes and QoL improvements are always welcome, but always be cautious when updating mods with large changes. It is better to keep in mind that every mod update has the potential to break something with pack. I cannot guarantee every update stability. So you should personally do your own research by checking their changelogs. 

* With the addition of keybind-based triggers that came along with `v2.3.0`. **PLEASE** check the EWC(ExtraWeaponCustomization) config and change the keybind to YOUR settings. I am aware that not everyone have keypads for their keyboards. 
    * Go to `Edit Config` within Thunderstore client -> Search for `ExtraWeaponCustomization.cfg` -> `Edit Config` -> Change keybinds 1 through 4 under `Keybind Settings` section

* Please let me know on my [Github](https://github.com/Heaveness/GTFriendlyO/issues) issue page if there are problems or if you have feedback. Thanks and have fun! 

### Mod Updates + Additions:
* Updated `Spectate` mod
* Updated `BetterBots` mod
* Updated `AmorLib` mod

### Weapon Additions:
* Updated `ExtraWeaponCustomization` mod
* Added `Ound9 gearpart II` mod by Ound9
* Removed the text, only the reload circle will be kept
* Added `3` new custom weapon!
* Bots cannot use the different weapon mode feature, so they will always default to mode 1 of the crossbow and medic gun. It is highly recommended you do not give weapons to bots that require nuance to use properly.
* **Hanaway Hunting Crossbow:**
* One of the most complex weapon added so far. Switch between three payloads: Regular, Napalm, and Foam bolts. Each payload has specific properties for different situations
    * Direct Damage: `10.0`
    * Clip Size: `1`
    * Max Ammo `20`
    * Reload Time: `3.5s`
    * Pierce Targets: `1.0`
    * Effective Range: `30.0m`
    * Hit Size: `+0.25m`
    * Stagger Multiplier: `1.5x`
    * Precision Multiplier: `3.25x`
    * Silenced, does not alert enemies
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-2.5m`
        * Crouching: `-1.0m`
        * Jumping: `5.0m`
    * Regular Bolts: (Default Keybind: KeypadPeriod[KeyConfig3])
        * Ballistics Type: `Fast Projectile Low Gravity`
        * Armor Pierce: `+10%`
        * Backstab Multiplier: `2.25x`
        * Recovers only `1.0` ammo per target killed
        * Max Delay requirement for ammo refund: `7.0s`
    * Napalm Bolts: (Default Keybind: KeypadEnter[KeyConfig1])
        * Ballistics Type: `Slow Projectile No Gravity`
        * Not Silenced, will alert enemies
        * Projectile Lifetime: `5.0s`
        * Shrapnel: `3` per `0.1s` with `0.75s` start delay
        * DoT Damage per tick: `14.0`
        * DoT Duration: `10.0s`
        * DoT Tick Rate: `2.0s`
        * DoT Stack Limit: `3`
        * Friendly Fire Multiplier: `0.5x`
        * Drops `1` Red Glowstick when the projectile times out or dies
    * Foam Bolts: (Default Keybind: KeypadPlus[KeyConfig2])
        * Ballistics Type: `Fast Projectile Mid Gravity`
        * Foam Time: `16.0s`
        * Foam Chance: `Override Guaranteed`
        * Foam Doors: `Yes`
        * Foam Door Requirements: `1` bolt if you hit the door after the first foam bolt hits
> Dev Note: The first "silent" weapon in the pack. To prevent this weapon's potential imbalance nature, the damage will be significantly more reliable in stealth scenarios. Its low max ammo capacity encourages players to shoot with purpose, as kills will refund only 1 ammo per target.
* **Techman Wisp Thrower:**
* An experimental entity that floats mid-air and attacks nearby targets until it bursts into several quills at the end of its life.
    * Max Ammo: `40`
    * Clip Size: `2`
    * No Reload, Clip Regen after `16.5s` delay after last firing
    * Clip Regen active while holstered
    * Launched Wisps will bounce off walls and objects before stopping to prevent dying on impact. Direct hits with entity will instantly kill the wisp.
    * Wisp Lifetime: `15.0s`
    * Wisp Direct Damage: `1.0`
    * Wisp Quill Damage: `5.0`
    * Wisp Quill Ricochet: `3`
    * Wisp Precision Multiplier: `1.1x`
    * Wisp Stagger Multiplier: `0.5x`
    * Wisp Friendly Fire Multiplier: `0.5x`
    * Wisp Targeting Priority: `Weakspots`
    * Wisp Launch Delay Attack: `1.0s`
    * Wisp Attack Speed: `2` Quills per `0.5s`
    * Wisp Death Quill Count: `10`
    * Wisp Death Quill Damage: `5.0`
    * Wisp Quill Max Range: `25.0m`
> Dev Note: An interesting weapon that has multiple uses. It has a good area denial which should pair well with trip mines and turrets. Also, it provides light which is great during EMP events or dark rundowns.
* **Van Auken Exp. Beam Rifle:**
* A manufactured copy of a patented prototype beam rifle in collabration with Techman Biotechnics.
    * Direct Damage: `1.0`
    * Reserve Ammo, no reload
    * Clip Regen up to `100` after Shot Delay
    * Max Ammo: `100`
    * Clip Size: `100`
    * Pierce Limit: `1` 
    * Fires `1` continuous beam costs `100` rounds
    * Damage increases continuous hitting a single target for the whole beam. 
        * Up to `1.5x` damage cap for normal shots as it stacks 1 at a time
        * Up to `2.0x` damage cap for weakspot shots as it stacks 2 at a time
        * Duration lasts `2.5s` then rapidly decays. Continued hits from the user will refresh the duration
    * Shot Delay: `2.0s`
    * DoT Damage: `1.0`
    * DoT Duration: `10.0s`
    * DoT Tick Rate: `2`
    * DoT Stack Limit: `100`
    * Shrapnel Count: `0.1`
    * Shrapnel Direct Damage: `0.1`
    * Shrapnel can contribute to DoT stacks
> Dev Note: Thanks to FE3, Dinorush, and EWC for the template to create this weapon. It's a concept that looks a little weird, but might have a niche usage. Does a significant amount of damage to single target, it is not recommended to spray fire as the base damage is very low.
### Tool Additions:
* Added `1` new custom tool!
* **Van Auken RYN0 Annihilator:**
* An extremely dangerous weapon from Van Auken's armory, capable of killing almost anything within the area. Truly a tool of destruction!
    * Direct Damage: `100`
    * Reserve Ammo, no reload
    * Max Ammo: `6`
    * Clip Size: `1`
    * Clip Regen after Shot Delay: `30.0s`
    * Charge Up Time: `2.5s`
    * Explosion Minimum Damage: `400.0`
    * Explosion Maximum Damage: `700.0`
    * Explosion Outer Radius: `10.0m`
    * Explosion Inner Radius: `5.0m`
    * Shrapnel Count: `60`
    * Shrapnel Damage: `5.0`
    * Stagger Multiplier: `5.0x`
    * Friendly Fire Multiplier: `0.1x`
    * Push based on shooting during standing/crouching/jumping:
        * Standing: `-14.0m`
        * Crouching: `-8.0m`
        * Jumping: `-18.0m`
> Dev Note: This is a meme weapon/tool and a little nod to one of the best sci-fi action-adventure game series ever made.

### Weapon Tweaks + Fixes:
* Medic Gun **Rework**:
    * Increased Max Delay Requirement for Ammo Refund from `0.5s` to `10.0s` (The maximum allowed delay in seconds between hitting the enemy and it dying.)
    * Decreased Baseline Projectile Count from `2` to `1` to prep for the different modes additions
    * Removed Last Hit kill requirement to refund ammo back
    * Increased Effective Range from `12.0m` to `20.0m`
    * Changed `Recoil` and `Accuracy` to be signifcantly more reliable
    * Increased Max Ammo from `100` to `110`
    * Players hit by healing darts should no longer constantly complain or grunt in pain during its duration
    * Reworked the function of this gun by adding a keybind trigger to switch between three modes with different effects.
    * Different modes can be stack individually with each other, but not with the same mode. For example: Stagger(Mode 2) + Armor Shred(Mode 3)
    * Mode 1: `Heal + Disinfection` Property
        * Activated by using specific keybind trigger(Default Keybind: KeypadPeriod[KeyConfig3])
        * Fires 2 bullets
        * Removed DoT Stagger Multiplier of `0.5x`
        * Applies to player targets:
            * Heal (stacks)
            * Disinfection (stacks)
        * Applies to enemy targets:
            * Toxin Damage(DoT)
                * Increased Precision Multiplier from `1.0x` to `1.2x`
                * Decreased Stagger Multiplier from `0.5x` to `0.0x`
            * Enemy Silence(CC stops non-boss tongue and projectile barrages)
    * Mode 2: `Speed + Stamina` Property
        * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
        * Fires only 1 bullet
        * Projectile Color: `Gold`
        * Buffs and Debuffs do not stack, it will only refresh duration
        * Applies to player targets:
            * Movement Speed buff of `+20%` over a duration of `10.0s` per bullet
            * Restore Stamina by `+20%` per bullet
        * Applies to enemy targets:
            * High Stagger Damage(DoT)
                * Decreased Total Damage from `25.0` to `1.0`
                * Decreased Precision Multiplier from `1.0x` to `0.0x`
                * Increased Stagger Multiplier from `0.0x` to `30.0x`
            * Enemy Silence(CC)
    * Mode 3: `Armor + Stamina` Property 
        * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])
        * Fires only 1 bullet
        * Projectile Color: `Purple`
        * Buffs and Debuffs do not stack, it will only refresh duration
        * Applies to player targets:
            * Armor Resistance of `+20%` over a duration of `10.0s` per bullet
            * Restore Stamina by `+20%` per bullet
        * Applies to enemy targets: 
            * Armor Shred debuff of `-20%` over a duration of `10.0s` per bullet
            * Weaker Toxin Damage(DoT)
                * Decreased Total Damage from `24.0` to `10.0`
                * Decreased Precision Multiplier from `1.0x` to `0.75x`
                * Increased Stagger Multiplier from `0.5x` to `1.0x`
            * Enemy Silence(CC)
> Dev Note: Here I am modifying the medic gun again. With these new changes, it will add a lot more complexity to the gun itself. Effectively making it the defacto "support" weapon.
* HMG:
    * Added `ThickBullet` property:
        * Added `0.2m` to projectile hitbox
* LMG:
    * Added `ThickBullet` property:
        * Added `0.2m` to projectile hitbox
* Reserve MP1:
    * Added `ThickBullet` property:
        * Added `0.15m` to projectile hitbox
* MP2:
    * Added `ThickBullet` property:
        * Added `0.15m` to projectile hitbox
* Drum Mag AR:
    * Increased Reload Time from `2.5s` to `2.8s`
    * Added `ThickBullet` property:
        * Added `0.15m` to projectile hitbox
> Dev Note: It should feel a little less punishing to spray into a crowd in a general area
* Full-Auto Light AR: **Rework**
    * Changed name from `Full-Auto Light AR` to `4-B Nade Launcher AR`
    * Changed `Scope` Part (improved the FOV & zoom of this scope)
    * Changed `Receiver` Part
    * Changed `Front` Part
    * Changed `Magazine` Part
    * Changed `Stock` Part
    * Decreased Hipfire Spread from `1.4x` to `1.0x`
    * Decreased Aimed Spread from `0.6x` to `0.4x`
    * Decreased Direct Damage from `6.5` to `5.0`
    * Decreased Clip Size from `30` to `20`
    * Increased Reload Time from `1.7s` to `2.2s`
    * Increased Max Ammo from `305` to `400`
    * Added `Explosive` property
        * Assault Rifle:
            * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
            * Changes Accuracy and Recoil data to `Bullpup`
            * Direct Damage: `4.0`
            * Burst Count: `4`
        * Nade Launcher:
            * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])
            * Changes Accuracy and Recoil data to `Rifle`
            * Direct Damage: `1.0`
            * Pulls from reserve ammo; does not use clip unless reserve is empty
            * Explosive Bullet Cost: `-15`
            * Explosion Minimum Damage(Inner): `25.0`
            * Explosion Maximum Damage(Outer): `45.0`
            * Explosion Outer Radius: `4.5m`
            * Explosion Inner Radius: `2.5m`
            * Stagger Multiplier: `2.0x`
            * Damages `Owner` and `Friendly`
            * Friendly Fire Multiplier: `0.75x`
            * Shrapnel Count: `10`
            * Shrapnel Damage: `5.0`
* Semi-Auto AR **Rework**
    * Changed name from `Semi-Auto Rifle` to `Semi/Full-Auto Rifle`
    * Changed `Scope` Part
    * Changed `Receiver` Part
    * Changed `Front` Part
    * Changed `Magazine` Part
    * Changed `Stock` Part
    * Changed `Flashlight` Part
    * Decreased Direct Damage from `8.1` to `7.5`
    * Increased Reload Time from `1.9s` to `2.6s`
    * Increased Clip Size from `20` to `45`
    * Increased Max Ammo from `203` to `295`
    * Added two modes: Switch between Semi-Auto and Full-Auto
        * Semi-Auto:
            * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
        * Full-Auto:
            * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])
> Dev Note: These two guns need a bit more love as they were basically two of the same. Also they sort of lacked identity compare to the other rifles.
* Foam Pistol:
    * Increased Glue Bubble Expansion Speed from `0.1x` to `0.25x`
    * Increased Armor Shred from `-20%` to `-30%`
    * Switched `ArmorShred` to `ShotModDebuff` property:
        * Applies `+30%` increased base damage(excluding precision & stagger) debuff on an enemy target for all sources
> Dev Note: With a lot of new options to foam targets, the Foam Pistol lost a lot of its place in the roster. So I am switching the armorshred to a "Increase Damage Taken" debuff on the target that is unique to this gun only.
* Exp. Smart Rifle:
    * Changed `Front` Part
    * Changed `Receiver` Part
    * Added Trail Color similar to Glow Color
    * Decreased Projectile Speed from `45.0m` to `25.0m` per second
    * Decreased Projectile Lifetime from `30.0s` to `10.0s`
    * Increased Minimum Projectile Distance from `10.0m` to `25.0m`
    * Added `Shrapnel` property:
        * A simple failsafe mechanism to lower the impact of orbiting projectiles
>Dev Note: Once a projectile times out around a target, a shrapnel similar to the original will spawn. This projectile will have a significantly stronger homing strength and angle which should properly hit its intended target more consistently. Orbiting projectiles might still get destroyed on a object or terrain.
* Heavy Revolver:
    * Changed `Stock` Part to prevent a log spamming issue.
* Tracker Pistol:
    * Changed `Front` Part(Scope Attachment)
* Tracker PDW:
    * Changed `Front` Part
    * Changed `Receiver` Part
* Tracker Rifle:
    * Changed `Front` Part
    * Changed `Receiver` Part
    * Changed `Magazine` Part
    * Increased Direct Damage from `35.1` to `40.1`
> Dev Note: While the Tracker Rifle is doing its job, I feel like its damage is still struggling to kill even smaller targets compare to DMRs. Also, I personally did not enjoy the look of the rifle.
* Hemorrhage HEL Rifle:
    * Increased Effective Range from `26.0m` to `35.0m`
    * Decreased Lock-on Angle Requirement from `3` to `2` degrees
    * Decreased Lock-on Time from `1.0s` to `0.5s`
    * Increased Lock-on Decay Time from `0.6s` to `0.8s`
> Dev Note: A very strong precision rifle, but its auto-aim feature felt very clunky. Hopefully this will make it more useable in chaotic moments.
* Pump-Action Shotgun:
    * Increased Max Ammo from `58` to `70`
* Triple Barrel Shotgun:
    * Increased Max Ammo from `71` to `81`
* Explosive Burst Rifle:
    * Changed `Receiver` Part
    * changed `Sight` Part
* Explosive Shotgun:
    * Changed `Receiver` Part
    * changed `Front` Part
* Explosive Cannon:
    * Increased Maximum Explosion Damage from `45.0` to `50.0`
    * Increased Minimum Explosion Damage from `35.0` to `40.0`
* W-Pen Sniper:
    * Changed `Front` Part
    * Changed `Receiver` Part
    * Changed `Sight` Part
    * Removed `Magazine` Part
    * Increased Push for both Standing & Jumping by `+2.0m`
    * Decreased Push for Crouching by `-1.0m`
* Nano Gauss Rifle:
    * changed `Receiver` Part
    * Increased Push for both Standing & Jumping by `+2.0m`
    * Decreased Push for Crouching by `-1.0m` 

### Class Tweaks:
* Updated `GTFuckingXP` mod
* Specialist:
    * Increased Fog Repeller/Turbine Power from `+80%` to `+100%`
    * Increased Initial Ammo Penalty from `-30%` to `-40%`
    * Decreased Ammo Cost Efficiency Penalty from `-30%` to `-20%`
> Dev Note: The Specialist should feel a lot more powerful against the Fog mechanics, but the constant buffs in recent patches should result in a nerf somewhere to counter balance.

* Paramedic:
    * Decreased Ammo Cost Efficiency Penalty from `-20%` to `-15%`

* Quartermaster:
    * Decreased Damage Penalty from `-50%` to `-30%`
    * Added Initial Tool Ammo Penalty of `-20%`

### Booster Tweaks:
* Added `PingableJunkieSyringes` mod by JarheadHME
    * Custom syringes weren't pingable which can cause some miscommunications
* Revive Spd. & Health `Muted` Booster:
    * Increased Revive Speed bonus from `+10%` to `+20%`
* Revive Spd. & Health `Bold` Booster:
    * Increased Revive Speed bonus from `+15%` to `+25%`
* Revive Spd. & Health `Aggressive` Booster:
    * Increased Revive Speed bonus from `+20%` to `+30%`
> Dev Note: The nature of revive speed works off the game's baseline 4.0s to 5.0s. So 45% is not worth a lot to risk taking all three boosters, now its 75% in the right condition which feel much more impactful.

### Tool Tweaks + Fixes:
* Updated `ExtraToolCustomization` mod
* Updated `DescriptiveWeaponStatShower` mod
    * Fixed custom turrets not having any stats shown in the tool select sceen
* Fog Repeller Consumable:
     * Decreased Minimum Consumable Loot Count from `5` to `4`
     * Decreased Maximum Consumable & Carry Limit Loot Count from `10` to `8`
* Search & Rescue Tool: **Improvement**
    * Increased Max Ammo from `30` to `40`
    * Removed Shell Casing ejection sound effects
    * Removed 3D Shooting sound effects for other players within the lobby
    * Changed aimed function to keybind-based modes
        * Mode 1:
            * Glowstick Launcher
            * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
            * Decreased Projectile Speed from `30.0m` to `25.0m` per second
        * Mode 2:
            * Fog Repeller Launcher
            * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])
            * Decreased Projectile Speed from `20.0m` to `15.0m` per second
> Dev Note: You should no longer hear your teammate's vanilla default gun shots when using these weapons, only the appropriate ones.
* 4-Burst Sentry:
    * Decreased Burst Delay from `2.0s` to `1.8s`
* Missile Sentry:
    * Added text description for traits
    * Fixed explosion not having friendly fire multiplier. *Oops...*
    * Increased Friendly Fire Multiplier from `-50%` to `-70%`
> Dev Note: I want to slightly lower the Burst turret's clunkiness to be a bit more reliable on maps that have tight corners.
* Exterminatus Flamer:
    * Removed Shell Casing ejection sound effects
    * Removed 3D Shooting sound effects for other players within the lobby
    * Changed `Scope` Part
    * Decreased Direct Damage from `1.0` to `0.5`
    * Decreased Projectile Glow Intensity from `0.25` to `0.05` (still bright, but not as before)
    * Increased Clip Regen Delay from `3.0s` to `5.0s`
> Dev Note: I removed the scope as it was pointless; replaced with iron sight. Also the long exposure to the flamethrower was giving me eye strain...

### Melee Tweaks + Fixes:
* Spear:
    * Increased Armor Pierce from `+15%` to `+20%`
    * Added `Push` Property when sprinting and charging heavy:
        * Sprint + Charge: `8.0m`
            * Based on charge amount starting from `50%`(4.0m) to `100%`(8.0m)
    * Added `ShotMod` Property when sprinting and charging heavy:
        * Increases damage of melee by `+30%`
            * Based on charge amount starting from `50%`(+15%) to `100%`(+30%)
> Dev Note: While I want to keep the Spear as a stealth melee. The knife is simply just too good at its job, and I do not want to nerf it. Instead I give the Spear more skill expression. You can use this lunge for a speed boost or kill a target quickly. Time it correctly and you can kill without alerting the room.
* Sledgehammer:
    * Fixed armor shred modifier not working correctly
    * Increased Armor Shred from `-30%` to `-40%`

### Syringe Fixes:
* Fixed issue with SyringeID and ItemID duplications when descending on a rundown
* Fixed multiple instances of same syringe distribution in the same rundon.

### Miscellaneous Fixes:
* Changed the wording on the pack's tagline description again
* Updated README.md file
* Updated CHANGELOG.md file
    * Fixed typos in CHANGELOG.md for v2.2.0
    * Removed old patch notes pre-v2.0 to save space for Thunderstore character limit. Check Github Repo for old changelog.

---

### v2.2.0

### Mod Updates + Additions:
* Added `WeaponIconPlus` mod by GTFOModding
* Added `Minimap` mod by HazardousMonkey
    * Located at Bottom Left section.
    * Change config settings to fit your needs.
    * Toggle default key: `M` (Recommend you either change your default Map key or this one. I use `TAB` for my map keybind)
    * Zoom Control: ALT + WheelDown/WheelUp
    * Recommended(optional) HUD size settings:
        * Compass: `80%`
        * Inventory: `100%` - `120%`
        * Chat: `90%`
        * Statusbar: `100%`
        * Subtitles: `100%`
        * Objective: `90%`
        * Intel: `90%`
* Updated `EnemyAnimationFix` mod
* Updated `MirrorWeapons` mod
* Updated `GTFuckingXP` mod
    * The in-game HUD for class information will properly hide itself during menus such as the map screen and ESC menu. No longer a wall of text will block teammate information.
* Updated `SpreadStartingAmmo` mod
* Updated `Amorlib` mod
* Updated `BetterBots` mod
* Updated `EEC H` mod
* Added `Spectate` mod by food
    * Spectate your teammates upon death(downed)

### Class Tweaks:
* Updated `GTFuckingXP` mod
    * Removed `DoubleJump` mod dependecy (You're free to remove this mod)
* Improved text organization on class selection screen to improve readability.
* HEL Diver:
    * Changed class description to match tone similar to the other B-Company Division members

* Specialist:
    * Increased Glue Strength & Efficiency from `+25%` to `+30%`
    * Increased Fog Repeller/Turbine Power from `+75%` to `+80%`
    * Increased Glowstick Power from `+150%` to `+175%`

* Field Technician:
    * Increased Initial Tool Ammo from `+40%` to `+50%`
    * Decreased Sentry Damage from `+50%` to `+40%`

### Weapon Tweaks:
* Updated `ExtraWeaponCustomization` mod
* Reworked Maximum Effective Range for all guns: (At this range, guns will do minimal damage)
    * All gun's maximum effective range has been either `decreased` or `increased` to be `double of the minimum effective range.` For example: minimum of `25.0m` will have `50.0m` maximum range.
    * You won't feel much difference on smaller rooms or maps. You might feel some difference on medium rooms. And you will feel especially on larger rooms.
    * Of course the exception are short-range guns(Shotguns and SMGs) will require players to fight in closer engagments. So to compensate, their low effective ranges were slightly increased.
* Improved Visual Lerp Distance for projectile guns for better visual feedback when shooting.
* Projectiles now trigger tripmines.
* Triple Barrel Shotgun:
    * Increased Effective Range from `5.0m` to `6.0m`
* Pump Action Shotgun:
    * Increased Effective Range from `6.0m` to `7.0m`
* Explosive Shotgun:
    * Increased Effective Range from `6.0m` to `7.0m`
* Reserve MP1:
    * Increased Effective Range from `5.0m` to `6.0m`
* MP2:
    * Increased Effective Range from `6.0m` to `7.0m`
* Hemorrhage Shotgun:
    * Increased Effective Range from `8.0m` to `9.0m`
* Foam Shotgun:
    * Increased Effective Range from `8.0m` to `9.0m`
* Tracker PDW:
    * Increased Effective Range from `9.0m` to `10.0m`
* Tracker Pistol:
    * Increased Effective Range from `11.0m` to `12.0m`
* Added `Hitmarker Cooldown` of `1.0s` for all DoT weapons to prevent excessive sound effects.
* Medic Gun:
    * Changed `Sight` Part
    * Changed `Receiver` Part
* Exp. Smart Rifle:
    * Changed `Sight` Part
* MP2:
    * Added `Sight` Part
    * Decreased Aim Spread from `0.5x` to `0.4x`
    * Increased Clip Size from `50` to `60`
    * Increased Max Ammo from `737` to `747`
* Explosive Shotgun:
    * Added `Shrapnel` property
        * Shrapnel Damage: `5.0`
        * Shrapnel Count per bullet: `2`
        * Shrapnel Pierce: `1.0`
* Triple Barrel Shotgun:
    * Added `Push` property when using `Aim` Trait
        * Standing/Crouching/Jumping: `-12.0m`
* Bolt Pistol:
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-2.0m`
        * Crouching: `-1.0m`
        * Jumping: `-4.0m`
* Heavy Revolver:
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-2.0m`
        * Crouching: `1.0m`
        * Jumping: `-4.0m`
* Nano Gauss Rifle:
    * Changed Explosion SFX to be a bit more squishy
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-5.0m`
        * Crouching: `-3.0m`
        * Jumping: `-10.0m`
* W-Pen Sniper Rifle:
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-4.0m`
        * Crouching: `-2.0m`
        * Jumping: `-8.0m`
* Reserve HMG:
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-0.05m`
        * Crouching: `0.0m`
        * Jumping: `-0.1m`
* LMG:
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-0.3m`
        * Crouching: `0.0m`
        * Jumping: `-0.5m`
* Explosive Shotgun:
    * Added `Push` property when shooting based on standing/crouching/jumping
        * Standing: `-3.0m`
        * Crouching: `-1.0m`
        * Jumping: `-6.0m`

### Tool Addition & Tweaks:
* Updated `ExtraToolCustomization` mod
* Changed name of `Autotek Tagged Sniper Turret` to `Autotek Bio-Tag Sniper Turret`
* Explosive Mine Deployer:
    * Changed name of `Krieg Homeland Defense` to `Krieg Homeland Defense Tool`
    * Decreased Max Ammo from `16` to `12`
    * Increased Minimum Effective Distance from `5.0m` to `6.0m`
    * Increased Maximum Effective Distance from `10.0m` to `12.0m`
    * Decreased Beam Length from `20.0m` to `12.0m` to match with its max effective range
    * Increased Placement Time from `1.0s` to `1.5s`
    * Increased Placement Cooldown from `1.0s` to `1.5s`
    * Increased Pickup Time from `1.0s` to `2.0s`
    * Increased Placement Range from `2.5m` to `6.0m`    
* Consumable Foam Tripmine:
    * Increased Firing Delay from `0.0s` to `0.1s`
    * Increased Minimum Effective Distance from `2.5m` to `3.0m`
    * Decreased Maximum Effective Distance from `12.0m` to `10.0m`
    * Decreased Beam Length from `20.0m` to `10.0m`
    * Decreased Foam Bubble Count from `17` to `15`
    * Increased Placement Range from `2.5m` to `3.0m`
    * Decreased Placement Cooldown from `2.0s` to `0.5s`
* Consumable Explosive Mine:
    * Increased Placement Range from `2.5m` to `3.0m`
* Advanced Bio Tracker:
    * Changed name from `Advanced Thermal Tracker` to `Techman Advanced Thermal Tracker`
    * Increased Equip Time from `1.0s` to `1.5s`
    * Decreased Aim Transition Time from `0.5s` to `0.25s`
* C-Foam Launcher:
    * Increased Max Ammo from `156` to `178`    
* 4-Burst Turret:
    * Increased Direct Damage from `4.6` to `5.2`
    * Decreased Shot Delay from `0.1s` to `0.05s`
* Shotgun Turret:
    * Increased Direct Damage from `5.9` to `6.0`
    * Increased Pellet Count from `7` to `8`
    * Decreased Shot Delay from `1.0s` to `0.75s`
    * Increased Max Ammo from `91` to `121`
* HMG Turret:
    * Increased Direct Damage from `1.6` to `1.7`
* Sniper Turret:
    * Increased Direct Damage from `85.5` to `90.5`
* Added four **NEW** tools! C-Foam Snare, Cave & Rescue, Exterminatus Flamer and Rocket Sentry
* **C-Foam Snare:(C-Foam Mine Deployer):**
    * Max Ammo: `15`
    * Firing Delay: `0.5s`
    * Minimum Effective Distance: `7.5m`
    * Maximum Effective Distance: `15.0m`
    * Beam Length: `15.0m`
    * Foam Bubble Count: `25`
    * Placement Range: `6.0m`
    * Placement Time/Cooldown/Pickup: `2.0s`
* **Mastaba Search & Rescue:**
    * Primary Fire mode: `Glowstick Launcher`
        * Costs: `1` ammo per shot
        * Will trigger `booster conditionals`
        * Effected by `boosters/class`
    * Secondary Fire mode: `Fog Repeller Launcher`
        * Costs: `2` ammo per shot
        * Will trigger `booster conditionals`
        * Effected by `boosters/class`
    * Max Ammo: `30`
    * Silence:
        * Wake Up Radius: `4.0m`
        * Alert Radius: `8.0m`
        * Alert Amount: `40%` (Sleepers awake at 100%)
* **Bio-Tag Rocket Turret:**
* There is no stat description for this turret because of issues with vanilla GTFO not playing nice with another mod. Unfortunately, I cannot fix it on my end. Please refer to the wiki for stats.
    * Direct Damage: `5.0`
    * Explosive Damage: `40.0`
    * Explosive Radius: `4.5m`
    * Shot Delay: `4.5s`
    * Max Ammo `20`
    * Shrapnel Count: `40`
    * Shrapnel Damage: `5.0`
    * Ballistic Type: `Homing Projectile`
    * Homing Priority: `Highest HP`
    * Homing Targeting: `Body`
    * Fires only at `Tagged` targets
    * Effective Range: `40.0m`
    * Friendly Fire: `50%` (Otherwise everyone will die)
    * Placement Time: `0.5s`
    * Pickup Time: `1.5s`
    * Deploy Time: `6.0s`
    * Scan Delay: `1.0s`
    * Scan Color: `Purple`
* **Exterminatus Flamer:**
    * Direct Damage: `1.0`
    * Multishot: `5.0x`
    * Bullet Hit Size: `+0.5m`
    * Pierce Targets: `2.0`
    * Stagger Multiplier: `10.0x`
    * Ballistics Type: `Slow Projectile Gravity`
    * Projectile Speed: `8.0m` per second
    * Projectile Lifetime: `5.0s`
    * Damage-Over-Time per Stack: `6.0`
    * DoT Stack Limit: `10`
    * DoT Duration: `10.0s`
    * Damage Interval: `2.0x`
    * DoT Stagger Multiplier: `1.0x`
    * DoT Friendly Multiplier: `0.5x`
    * Cannot Reload, Clip Regen from Reserves after Firing
    * Clip Regen: `5.0` per second
    * Clip Regen Delay: `3.0s`
    * Max Ammo: `1000`
    * Clip Size: `100`
    * Explosion on Death, applies 1 stack of DoT
    * Explosion Damage: `1.0`
    * Explosion Radius: `3.5m`
    * Explosion Stagger Multiplier: `5.0x`
    * ChargeUp Time: `0.4s`
    * Slow Fire Rate, must Accelerate to increase Fire Rate
    * Flames will ricochet off of walls at an extremely slow speed
    * Flames will "stay" on the ground up to a few seconds which will apply damage

### Melee Tweaks:
* Sledgehammer:
    * Increased Armor Shred Duration from `4.0s` to `4.5s`

### Booster Tweaks:
* Changed text from `99 Uses Left` to `Infinite Uses`
* Initial Main/Special Ammo `Muted` Booster:
    * Fixed boosters showing the wrong value of `14%`
* Initial Main/Special Ammo `Aggressive` Booster:
    * Increased Main/Special ammo bonus from `25%` to `35%`
* Initial Tool Ammo `Muted` Booster:
    * Increased Tool ammo bonus from `10%` to `15%`
* Initial Tool Ammo `Aggressive` Booster:
    * Increased Tool ammo bonus from `20%` to `35%`
* Regen Cap/Speed `Bold` Booster:
    * Changed Condition from `Human Proximity` to `Glowstick Radius`
* Tripmine Damage `Bold` Booster:
    * Changed Condition from `Holding Tool` to `Human Proximity`

### Miscellaneous Tweaks + Fixes:
* Moved Minimap location
* Fixed various issues:
    * Fixed errors of duplicate weapon gear parts
    * Fixed Gear Category duplicate data blocks
    * Fixed errors with Template.json in EWC being loaded
    * Fixed errors regarding reserve shotgun and explosive shotgun's spread being not considered
* Updated README.md file
    * Added more tools into the tool section
    * Improved the tagline of the modpack to better describe the modpack's vision
* Removed old Dev Notes up v2.1.0 in CHANGELOD.md to make space. Old changelog with all dev notes will be kept up in Github repo.

---

### v2.1.0

### Mod Updates:
* Updated `EnemyAnimationFix` mod
* Updated `AmorLib` mod
* Updated `ModifierAPI` mod
* Updated `ExtraWeaponCustomization` mod
* Updated `ExtraSyringeCustomization` mod
    * Removed `MovementSpeedAPI` mod
* Added `StrongerPlayer` mod by Chaxi
    * Ability to sprint while holding onto objective items such as Fog Turbines, Battery Cells, and other large objects that require both hands.

### Enemy Tweaks:
* Stalker(Snatcher):
    * Decreased Health from `3500` to `700`
    * Decreased Damage Until React from `2000` to `500`
    * Decreased Bodypart Health from `2500` to `600`
    * Increased Initial Held Damage from `0.0` to `5.0`
    * Decreased Tag Time from `30.0s` to `20.0s`
    * Increased Dash Cooldown from `5.0s` to `13.0s`
    * Increased Runaway Duration from `5.0s` to `13.0s`
    * Increased Dash Speed Modifier from `1.0x` to `2.0x`
* Kraken(Boss):
    * Decreased Health from `9000` to `7000`
    * Increased Bodypart Health from `1800` to `2000`
* Tank:
    * Decreased Glue Tolerance from `25.0` to `20.0`

### Weapon Tweaks:
* Nano Gauss Rifle:
    * Decreased Shrapnel(Gobules) count from `20.0` to `10.0`
    * Increased Shrapnel(Gobules) damage from `2.0` to `4.0`

### Misc. Tweaks:
* ChatterReborn:
    * Removed banter whenever someone carried the Fog Turbine.

---

### v2.0.10

* Emergency Hotfix:
    * Updated `MovementSpeedAPI` mod 
    * Added `MovementSpeedAPI` mod back into the manifest

---

### v2.0.9

### Mod Update & Fixes:
* Updated `ExtraWeaponCustomization` mod
* Updated `ExtraToolCustomization` mod
* Updated `GTFuckingXP` mod
* Added `EnemyAnimationFix` mod by Dinorush
    * Fixes several enemy bugs for both clients and host regarding their animations and attack behavior. 
* Added `DMRReloadFix` mod by randomuserhi
    * Fixes an annoying bug when reloading guns that leaves 1 bullet missing in the magazine.
* Added `DoorEnemyFixUpdated` mod by Dinorush
    * Fixes Tripmines and C-Foam touching enemies through closed doors which will cause them to trigger prematurely and waste the resource. 
* Added `ReDownFix` mod by Dinorush
    * Fixes clients getting downed from taking any damage shortly after a revive. This is to prevent players from getting killed immediately after a successful revive caused by the long animation.
* Added `PierceBugFix` mod by tru0067
    * Fixes piercing so that piercing shots hit the advertised number of enemies. Originally piercing beyond five were ignored by the system and some enemies used up more than one piercing; effectively decreasing their utility.

### Class Tweaks:
* Added `Melee Attack Speed` modifier to certain classes.
* Marine:
    * Increased Bleed Resistance from `+70%` to `+90%`
    * Increased Projectile Armor boon from `+30%` to `+40%`
    * Added `Melee Attack Speed` property
        * Class decreases `Melee Attack Speed` by `-50%`
* Shock Trooper:
    * Fixed typos within the text description
    * Fixed class not showing the Health Regen bonus when in-game
    * Removed `Melee Damage` property of `+20%`
    * Added `Melee Attack Speed` property
        * Class increases `Melee Attack Speed` by `+30%`
* Abhuman:
    * Increased Melee Damage from `+75%` to `+100%`
    * Increased Terminal & Sentry CPU penalty from `-50%` to `-70%`
    * Added `Melee Attack Speed` property
        * Class decreases `Melee Attack Speed` by `-30%`
* Deprived:
    * Increased Projectile Armor penalty from `-50%` to `-60%`
    * Added `Melee Attack Speed` property
        * Class increases `Melee Attack Speed` by `+50%` 

### Booster Tweaks:
* Initial Main/Special Ammo Boosters:
    * Increased Muted Ammo Bonus from `+10%` to `+15%`
    * Increased Aggressive Ammo Bonus from `+20%` to `+25%`
* Bold Melee Boosters:
    * Changed Booster Condition from `Low Health` to `Glowstick Radius`
    * Changed Booster Condition from `High Health` to `Fog Repeller Radius`

### Melee Tweaks:
* Sledge Hammer:
    * Decreased Stamina Cost while in combat from `35%` to `30%` per Heavy swing.
* Spear:
    * Decreased Stamina Cost while in combat from `35%` to `25%` per Heavy swing.
    * Decreased Stamina Cost while out of combat from `30%` to `25%` per Heavy swing.
    * Decreased Stamina Cost while in combat from `25%` to `20%` per Light swing.

### Misc. Fixes:
* Fixed wording in `v2.0.7` changelog that stated Striker Giant's new Body Part Health was `1.0` when it should have been `175.0`.

---

### v2.0.8

* Emergency Hotfix:
    * Fixed an error with one of the gun's properties.

---

### v2.0.7

### Weapon Tweak:
* Updated `ExtraWeaponCustomization` mod
* Medic Gun:
    * Increased Dart Duration from `9.0s` to `9.5s` (To prevent potential loss of time from packet loss)
    * Added `Disinfect` property
    * Each dart will disinfect players for `0.31%` per second for a duration of `9.5s` 

### Enemy Body Part Health Tweaks:
* Striker:
    * Decreased Body Part Health from `24.0` to `20.0`
* Nightmare Striker:
    * Decreased Body Part Health from `51.5` to `31.5`
* Striker Charger:
    * Increased Body Part Health from `12.0` to `22.0`
* Striker Giant:
    * Decreased Body Part Health from `450.0` to `175.0`
* Nightmare Striker Giant:
    * Decreased Max Health from `900.0` to `600.0`
    * Decreased Hit Reaction Threshold from `960.0` to `200.0`
    * Decreased Body Part Health from `900.0` to `250.0`
* Nightmare Needler:
    * Decreased Body Part Health from `27.5` to `20.5`
* Nightmare Scout:
    * Decreased Body Part Health from `120.0` to `80.0`
* Stalker:
    * Decreased Max Health from `4000.0` to `3500.0`
    * Decreased Body Part Health from `4000.0` to `2500.0`
    * Decreased Tag Time from `60.0s` to `30.0s`

### Enemy Fixes & Tweaks:
* Removed Projectile Settings from EEC to prevent issues with enemy abilities.
* Nightmares Variants:
    * Decreased Projectile Infection Rate from `1%` to `0.5%`
* Enemy Bleed Effect:
    * Enemy Bleed NO longer stacks; continued application can refresh active bleed duration
    * Fixed Bleed doing the wrong amount of damage
    * Added Bleed properties to Scouts(except Nightmare Scouts)
    * Increased Bleed Damage from `0.4%` to `2%`
    * Increased Damage Interval from `1.0s` to `2.0s`
    * Increased Bleed Duration from `5.0s` to `10.5s`
* Flyer:
    * Decreased Explosion Minimum Range from `2.5m` to `2.0m`
    * Decreased Explosion Maximum Range from `5.0m` to `4.0m`
* Shadow:
    * Decreased Infection Fog Rate from `0.5%` to `0.3%` per second
    * Decreased Infection Fog Duration from `35.0s` to `30.0s` 

### Melee Fixes:
* Sledgehammer:
    * Fixed Sledgehammer Armor Shred not working because of invalid trigger setting.

### Misc Fixes:
* Minor format improvements to README file.

---

### v2.0.6

### Emergency Hotfix:

* Fixed some changes not included in v2.0.5 by accident.

---

### v2.0.5

### Mod Additions:
* Added `SpreadStartingAmmo` mod by Dinorush
* Ammo is spread from a pool given to players on startup based on how many players are present. If a player/bot joins then the pool is reduced to accommodate the new player(s), dismissing the slot will not refund the lost ammo from the distribution.
    * 1 Player: 4x ammo
    * 2 Players: 2x ammo 
    * 3 Players: 1.33x ammo
    * 4 Players: 1x ammo (Bots count as players)

### Weapon Fixes & Tweaks:
* Bolt Pistol:
    * Increased Precision Multiplier from `0.6x` to `0.7x`
    * Increased Stagger Multiplier from `1.5x` to `2.0x`
* Tracker Rifle:
    * Increased Direct Damage from `28.1` to `35.1`
    * Increased Precision Multiplier from `1.2x` to `2.0x`
    * Decreased Stagger Multiplier from `2.0x` to `1.5x`
* Nano Gauss Rifle:
    * Increased Direct Damage from `50.5` to `55.5`
    * Increased Projectile Speed from `60` to `65`
    * Increased Projectile Hit Size by `0.2m`
    * Increased Precision Multiplier from `2.0x` to `4.0x`
    * Increased Stagger Multiplier from `1.5x` to `2.0x`
* Sniper Rifle:
    * Increased Armor Pierce from `10%` to `20%`
    * Increased Precision Multiplier from `4.0x` to `6.0x`
* Reserve HMG:
    * Increased Stagger Multiplier from `1.8x` to `2.0x`
    * Once again trying to fix this gun's first person model after fixing the third person model from a previous patch.

### Turret Fixes & Tweaks:
* Added "More effective against Tagged" for all turrets.
* Fixed wrong values for Stagger Multiplier against tagged targets.
* Sniper Turret:
    * Increased Tagged Stagger Multiplier from `1.0x` to `1.1x`
* Burst Turret:
    * Increased Burst Delay from `1.0s` to `2.0s`
    * Decreased Shot Delay from `0.5s` to `0.1s`
    * Increased Tagged Stagger Multiplier from `1.0x` to `1.15x`
* HMG Turret:
    * Increased Tagged Stagger Multiplier from `1.0x` to `1.25x`
* Shotgun Turret:
    * Decreased Shot Delay from `1.3s` to `1.0s`
    * Increased Tagged Stagger Multiplier from `1.0x` to `1.2x`

### Tool Fixes & Tweaks:
* C-Foam Launcher:
    * Increased Max Ammo Capacity from `100` to `156`
* Mine Deployer:
    * Increased Radius from `2.5m` to `3.0m`
    * Increased Minimum Distance from `3.0m` to `5.0m`
    * Decreased Maximum Distance from `15.0m` to `10.0m`
    * Increased Minimum Explosive Damage from `30` to `75`
    * Increased Maximum Explosive Damage from `100` to `125`
    * Increased Stagger Force from `1200` to `1300`
    * Increased Arming Time from `0.3s` to `1.0s`
    * Increased Placement Time from `0.4s` to `1.0s`
    * Increased Pickup Time from `0.4s` to `1.0s`
* Consumable Mine:
    * Increased Radius from `2.5m` to `3.0m`
    * Increased Minimum Distance from `1.5m` to `3.0m`
    * Decreased Maximum Distance from `15.0m` to `10.0m`
    * Increased Minimum Explosive Damage from `15` to `40`
    * Increased Maximum Explosive Damage from `60` to `75`
    * Increased Stagger Force from `800` to `900`
    * Increased Arming Time from `0.3s` to `0.5s`
    * Increased Placement Time from `0.4s` to `0.5s`
    * Increased Pickup Time from `0.4s` to `0.5s`
    * Decreased Placement Cooldown from `1.0s` to `0.5s`

### Enemy Fixes & Tweaks:
* Added underline text for all tagged enemies to help separate the name and healthbar for visual clarity.
* Shadows:
    * Fixed this variant not creating infected fog spheres on death when hibernating.
* Striker Giants:
    * Increased Body Part Health from `300` to `450`
    * Increased Weakspot Damage Multiplier from `0.4x` to `0.6x`

### Class Fixes:
* Quartermaster:
    * Fixed a typo wrong info text regarding movement speed while in-game.

---

### v2.0.4

### Updates:
* Updated `ExtraWeaponCustomization` mod.
* Updated `GTFuckingXP` mod.
* Updated README file.

### Weapon Fixes:
* Foam Pistol:
    * Fixed the improper armor shred values during foam. It should properly apply the `-20%` armor debuff(increasing damage from most sources).
* Medic Gun:
    * Added `Ammo Mod` property
    * Killing an enemy with the venom darts will restore `1.0` ammo back into the reserve.
        * Does **NOT** refund more than 1 dart per kill.
* Fixed HEL Revolver and Heavy Revolver's ricochet bullet using the old version of the revolver's stat.
* HEL Revolver:
    * Decreased Ricochet's Direct Damage from `13.6` to `5.0`   
    * Increased Ricochet's Precision Multiplier from `1.1x` to `3.5x` (Lower than baseline by 0.75x)
    * Decreased Ricochet's Stagger Multiplier from `1.0x` to `0.65x` (Lower than baseline by 0.2x)
    * Decreased Ricochet's Effective Range from `50.0m` to `20.0m`
* Heavy Revolver:
    * Decreased Ricochet's Direct Damage from `35.9` to `10.0` 
    * Increased Ricochet's Precision Multiplier from `1.1x` to `5.5x` (Lower than baseline by 0.75x)
    * Decreased Ricochet's Stagger Multiplier from `1.0x` to `0.7x` (Lower than baseline by 0.2x)
    * Decreased Ricochet's Effective Range from `50.0m` to `20.0m`

### Melee Fixes & Tweaks:
* Fixed melee weapons using the wrong noise levels:
    * 0: Wakes up sleepers in 7m from hitting locks or the ground.
    * 1: Wakes up sleepers in 4m from hitting locks or the ground. Also has reduced chance to trigger long range aggro
        * Knife: 1
        * Spear: 1
        * Sledgehammer: 0
        * Bat: 0
* Sledgehammer:
    * Removed `Armor Pierce` property
    * Added `Armor Shred` property
        * Applies armor shred of `-30%` for `4.0s` on hit; non-stackable
        * Requires charge up bar of `40%` to acquire `half` of the armor shred modifier. 
        * Requires charge up bar of `100%` to acquire `full` armor shred debuff. 
        * Any charge in-between will give varying armor shred values.
* Knife:
    * Increased Light Backstab Multiplier from `2.0x` to `2.1x`
    * Increased Heavy Backstab Multiplier from `2.5x` to `2.6x`
    * Decreased Total DoT Damage from `6.0` to `5.0`
    * Decreased stack limit from `unlimited` to `4`
    * Increased DoT timer from `3.0s` to `4.0s` (takes a little longer to reach total damage)
* Spear:
    * Removed can hit multiple targets, unintentional.
    * Increased Armor Pierce bonus from `+10%` to `+15%`
* Bat:
    * Decreased Explosion Damage from `10.0` to `5.0`
    * Increased Explosion Stagger Multiplier from `1.5x` to `3.5x`

---

### v2.0.3

* Dev Note: If you have any feedback on the modpack, please do not hesitate to comment in the github issue tab [here](https://github.com/Heaveness/GTFriendlyO/issues)!

### Mod Updates:
* Updated `ExtraWeaponCustomization` mod.
* Updated `GTFuckingXP` mod.
* Removed `SpreadStartingAmmo` mod <= **IMPORTANT**

### Enemy Tweaks:
* Striker Giant:
    * Increased Body Part Health from `200` to `300`

### Weapon Fixes:
* Reserve HMG:
    * Fixed third person model of the gun being upside down.
* HEL Revolver:
    * Fixed HEL Revolver not having proper reload animations.
    * Changed `Stock Part`
* Explosive Cannon:
    * Decreased ChargeUp Time from `0.9s` to `0.8s`
    * Fixed Aimed Acceleration modifier not working. It should properly fire quickly again.

---

### v2.0.2

### Tweaks:
* Reserve MP1:
    * Increased Stagger Multiplier from `2.0x` to `3.5x`

### Syringe Fixes:
* Added wiki page for Syringe Information.
* Fixed Advanced Slow Healing Syringe using the wrong healing value of `0.2` instead of `0.4`
    * Changed healing value from `0.2` to `0.4` (total health of `24.0`)
* Fixed Masterful Slow Healing Syringe using the wrong name.
    * Proper Name: Antibiotic-IX-REC Syringe

### Fixes:
* Added more dialogue options from `ChatterReborn` mod for specific situations:
    * Fog Turbine
    * Callout Teammates (ping teammates)
    * Keycard Pickup
    * Random Comments
* Fixed Triple-Barrel Description. (it wasn't suppose to have numbers)
* Fixed Single Slugger Description. (Forgot to mention faster reload speed on kill bonus)
* Fixed typos in README file
* Fixed typos in CHANGELOG file

---

### v2.0.1

### Class Tweaks:
* Courier:
    * Increased Infection/Explosion/Bullet/Bleed Res. penalty from `70%` to `80%`
    * Removed Initial Tool Ammo bonus.
* Field Technician:
    * Decreased Sentry CPUs from `+30%` to `+20%`
* Abhuman:
    * Decreased Bioscan Speed & Recharge Speed penalty from `-50%` to `-40%`

### Enemy Tweaks:
* Striker Giant:
    * Increased Max Health from `400` to `450`
* Needler Giant:
    * Increased Max Health from `275` to `300`
* Scout:
    * Changed Scout feeler animation (it should stay standing even when retracting)
    * Decreased Movement Detection Distance from `8.0m` to `1.0m` (allows players to get closer without immediately triggering reactionary feelers)
    * Decreased Minimum Weapon Detection from `10.0m` to `5.0m` (easier to stealth kill around target without 100% alerting)
    * Increased Max Tentacle count from `50` to `60` (more feelers)
    * Decreased Tentacles Speed from `10.0m` to `2.5m` per second (slower than Vanilla's 7.5m)
    * Decreased Time to Retract Tentacles from `2.5s` to `1.0s` (faster to finish retracting)
    * Decreased Max Distance of Tentacles from `60.0m` to `40.0m` (shorter feelers)

### Weapon Tweaks & Fixes:
* Removed Relax position for all guns to prevent some animation issues.
* Foam Pistol:
    * Increased Foam & Armor Shred Duration from `6.0s` to `10.0s`
    * Decreased Armor Shred debuff from `-30%` to `-20%`
* HEL Shotgun: **Rework**
    * Renamed Buckland HEL Shotgun to `Buckland Foam Shotgun`
    * Fixed accidental mistake of this gun using (HEL) booster effect, it should say it is using Shotgun modifier.
    * Foam Shotgun will have two different stats based on hipfire and aim mode.
    * Hipfire: Shotgun
        * Fire Mode: Semi-Auto
        * Direct Damage: `9.5`
        * Pellet Count: `6`
        * Effective Range: `8.0m`
        * Magazine Size: `8`
        * Max Ammo Capacity: `66`
        * Reload Time: `2.0s`
        * Ammo Cost per shot: `-1`
        * Pierce Limit: `1`
    * Aimed: Foam
        * Fire Mode: Semi-Auto
        * Foams on Enemy Hit only
        * Foam Duration: `5.0s`
        * Foam does NOT barricade doors
        * Ammo Cost per shot: `-2`
        * Movement Speed of `+20%`
        * Speed Duration: `5.0s`
    * Changed `Front Part`
    * Changed `Receiver Part`
    * Changed `Sight Part` 
* Single Slugger:
    * Changed `Front Part`
    * Changed `Sight Part`
* LMG:
    * Decreased Direct Damage from `8.2` to `8.0`
    * Increased Magazine Size from `70` to `100`
    * Increased Max Ammo Capacity from `413` to `500`
* Reserve HMG:
    * Decreased Direct Damage from `4.6` to `4.0`
    * Increased Stagger Multiplier from `1.7x` to `1.8x`
    * Increased Max Ammo Capacity from `885` to `1000`
    * Changed `Magazine Part`
    * Changed `Stock Part`
* Heavy Rifle:
    * Changed `Sight Part`
    * Increased Direct Damage from `3.0` to `3.1`
    * Increased Magazine Size from `60` to `70`
    * Increased Max Ammo Capacity from `452` to `528`
* Burst Cannon:
    * Fixed the gun having the wrong temporary stats while aiming.
* Triple Barrel Shotgun:
    * Decreased Direct Damage from `5.0` to `4.0`
    * Increased Reload Time from `1.4s` to `1.5s`
    * Decreased Equip Time from `0.33s` to `0.2s`
    * Added `Melee Damage` modifier
        * Grants non-stacking melee buff of `+25%` 
        * Over a duration of `3.0s`
        * Activates on `Enemy Hit` only

### Melee Tweaks:
* Sledgehammer:
    * Decreased Max Charge Time for Heavy Attack from `3.0s` to `2.7s`
* Spear:
    * Decreased Max Charge Time for Heavy Attack from `3.7s` to `3.2s`

### Player Tweaks:
* Increased the `AmmoStandardInitial` & `AmmoSpecialInitial` from `250` to `275` (Starting Ammo for Main and Special weapon slots)

### Misc.
* Updated `ExtraWeaponCustomization` mod
* Updated `MovementSpeedAPI` mod
* Updated `ExtraEnemyCustomization` mod
* Updated `ExtraSyringeCustomization` mod

---

### v2.0.0 Final Major Update

### Weapon Rework(Precision & Stagger Multiplier):
* The vanilla GTFO baseline precision is 0.74x because it is added on top of enemy's weakspot multipliers. Each enemy has their own weakspot multiplier which I will not provide here, they haven't changed from vanilla values.

**Baseline Precision:** 0.74x --> 0.75x

**Baseline Stagger:** 1.0x --> 1.0x

| Weapon Name                 | Precision (Old) | Precision (New) | Stagger (Old) | Stagger (New)  |
|-----------------------------|:---------------:|:---------------:|:-------------:|:--------------:|
| Tracker Pistol              | 0.87x           | 0.65x           | 1.50x         | 2.00x          |
| Foam Pistol                 | 0.87x           | 0.50x           | 1.00x         | 10.00x*        |
| HEL Revolver                | 0.74x           | 4.25x*          | 1.00x         | 0.85x          |
| MP2                         | 0.74x           | 0.85x           | 1.00x         | 0.50x          |
| Reserve MP1                 | 0.74x           | 0.65x           | 2.00x         | 2.00x          |
| 5-B Bullpup                 | 1.00x           | 0.75x           | 1.00x         | 1.30x          |
| Hemostasis Medic Gun        | 1.00x           | 0.65x           | 1.00x         | 10.00x*        |
| Tracker PDW                 | 0.74x           | 0.65x           | 1.00x         | 1.50x          |
| Heavy SMG                   | 0.80x           | 0.70x           | 1.00x         | 1.20x          |
| 3-B Carbine                 | 0.74x           | 0.85x           | 1.00x         | 1.00x          |
| DMR                         | 0.97x           | 1.00x           | 1.00x         | 0.65x          |
| Double-Tap                  | 0.95x           | 0.75x           | 1.00x         | 1.40x          |
| Heavy Rifle                 | 0.80x           | 0.65x           | 1.00x         | 1.30x          |
| Explosive Burst Rifle       | 1.00x           | 0.65x           | 1.20x         | 1.50x          |
| Assault Rifle               | 0.87x           | 0.90x           | 1.75x         | 0.80x          |
| Triple-Barrel               | 0.74x           | 0.75x           | 2.00x         | 2.00x          |
| HEL Shotgun(Name Changed)   | 0.74x           | 0.75x           | 2.00x         | 2.00x          |
| Single Slugger              | 1.50x           | 1.60x           | 1.00x         | 0.80x          |
| AR-30                       | 0.80x           | 0.90x           | 1.00x         | 0.90x          |
| Experimental Smart Rifle    | 1.30x           | 1.40x           | 0.50x         | 0.50x          |
| Pump-Action                 | 1.00x           | 0.75x           | 2.00x         | 2.50x          |
| Hemorrhage Shotgun          | 0.88x           | 0.75x           | 2.00x         | 2.00x          |
| Explosive Shotgun           | 0.73x           | 0.45x           | 2.00x         | 2.00x          |
| Choke Shotgun               | 1.00x           | 0.90x           | 2.00x         | 1.50x          |
| Heavy Revolver              | 0.95x           | 6.25x*          | 1.00x         | 0.90x          |
| LMG                         | 0.74x           | 0.80x           | 1.00x         | 0.80x          |
| Reserve HMG                 | 0.74x           | 0.65x           | 1.45x         | 1.70x          |
| Explosive Cannon            | 0.73x           | 0.55x           | 1.00x         | 1.75x          |
| Hemorrhage HEL              | 0.80x           | 1.00x           | 1.00x         | 0.80x          |
| Bolt Pistol                 | 0.74x           | 0.60x           | 1.00x         | 1.50x          |
| Tracker Rifle               | 1.30x           | 1.20x           | 1.00x         | 2.00x          |
| Sniper Rifle                | 4.00x           | 4.00x           | 3.00x         | 3.00x          |
| Nano Gauss Rifle            | 1.10x           | 2.00x           | 1.00x         | 1.50x          |
* Certain weapons have a reason for the exaggerated multiplier values. Please check the **Weapon Tweaks** section below this patch(*).

### Weapon Rework(Effective Range):
* Changes made to effective range to better reflect a weapon's role in conjunction with their class roles.

| Weapon Name               | Effective Range (Old) | Effective Range (New) |
|---------------------------|:---------------------:|:---------------------:|
| Tracker Pistol            | 9.0m                  | 11.0m                 |
| Foam Pistol               | 7.0m                  | 10.0m                 |
| HEL Revolver              | 10.0m                 | 13.0m                 |
| MP2                       | 6.0m                  | 7.0m                  |
| Reserve MP1               | 6.0m                  | 5.0m                  |
| 5-B Bullpup               | 10.0m                 | 18.0m                 |
| Hemostasis Medic Gun      | 12.0m                 | 12.0m                 |
| Tracker PDW               | 6.0m                  | 9.0m                  |
| Heavy SMG                 | 9.0m                  | 14.0m                 |
| 3-B Carbine               | 10.0m                 | 22.0m                 |
| DMR                       | 50.0m                 | 35.0m                 |
| Double-Tap                | 40.0m                 | 25.0m                 |
| Heavy Rifle               | 10.0m                 | 17.0m                 |
| Explosive Rifle           | 30.0m                 | 20.0m                 |
| Assault Rifle             | 22.0m                 | 23.0m                 |
| Triple-Barrel             | 6.0m                  | 5.0m                  |
| HEL Shotgun               | 5.0m                  | 6.0m                  |
| Single Slugger            | 30.0m                 | 25.0m                 |
| AR-30                     | 20.0m                 | 21.0m                 |
| Experimental Smart Rifle  | 10.0m                 | 15.0m                 |
| Pump-Action               | 5.0m                  | 6.0m                  |
| Hemorrhage Shotgun        | 8.0m                  | 8.0m                  |
| Explosive Shotgun         | 5.0m                  | 6.0m                  |
| Choke Shotgun             | 16.0m                 | 14.0m                 |
| Heavy Revolver            | 20.0m                 | 21.0m                 |
| LMG                       | 16.0m                 | 20.0m                 |
| Reserve HMG               | 16.0m                 | 18.0m                 |
| Explosive Cannon          | 20.0m                 | 20.0m                 |
| Hemorrhage HEL            | 16.0m                 | 26.0m                 |
| Bolt Pistol               | 25.0m                 | 18.0m                 |
| Tracker Rifle             | 40.0m                 | 45.0m                 |
| Sniper Rifle              | 80.0m                 | 60.0m                 |
| Nano Gauss Rifle          | 40.0m                 | 50.0m                 |

### Weapon Rework(Hipfire/Aimed Spread):
* Changes made to both hipfire spread and aimed spread for all guns to further differentiate between precision and spray weapons. Some weapons might be an exception to this rule.
    * Moderately increased Aimed spread for all spray guns(Scatter).
        * Slightly decreased Hipfire spread.
    * Moderately increased Hipfire spread for all precision guns(Stabilized). 
        * Slightly increased Aimed Spread for some guns.
* Added Weapon Class definition for each gun:
    * All Spray guns are classified as `Scatter`
    * All Precision guns are classified as `Stabilized`
    * All Mixed guns are classified as `Hybrid`
    * Any Support guns are classified as `Utility`

| Weapon Name              | Hipfire (Old) | Hipfire (New) | Aimed (Old) | Aimed (New) | Class      |
| ------------------------ | :-----------: | :-----------: | :---------: | :---------: | :--------: |
| Tracker Pistol           | 1.00x         | 1.30x         | 0.00x       | 0.05x       | Stabilized |
| Foam Pistol              | 0.50x         | 0.40x         | 0.00x       | 0.00x       | Utility    |
| HEL Revolver             | 2.00x         | 2.50x         | 0.00x       | 0.15x       | Stabilized |
| MP2                      | 1.90x         | 1.40x         | 0.00x       | 0.50x       | Scatter    |
| Reserve MP1              | 2.10x         | 1.70x         | 0.00x       | 0.80x       | Scatter    |
| 5-B Bullpup              | 2.50x         | 2.00x         | 0.00x       | 1.00x       | Scatter    |
| Hemostasis Medic Gun     | 0.05x         | 0.10x         | 0.00x       | 0.00x       | Utility    |
| Tracker PDW              | 1.25x         | 1.00x         | 0.00x       | 0.60x       | Scatter    |
| Heavy SMG                | 2.00x         | 2.30x         | 0.00x       | 0.30x       | Stabilized |
| 3-B Carbine              | 1.00x         | 1.30x         | 0.00x       | 0.40x       | Hybrid     |
| DMR                      | 0.50x         | 1.00x         | 0.00x       | 0.10x       | Stabilized |
| Double-Tap               | 2.50x         | 2.00x         | 0.00x       | 0.50x       | Hybrid     |
| Heavy Rifle              | 2.00x         | 1.60x         | 0.00x       | 0.90x       | Scatter    |
| Explosive Burst Rifle    | 2.50x         | 2.00x         | 0.00x       | 0.60x       | Hybrid     |
| Assault Rifle            | 1.00x         | 1.50x         | 0.00x       | 0.30x       | Stabilized |
| Triple-Barrel*           | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Scatter    |
| HEL Shotgun*             | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Scatter    |
| Single Slugger*          | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Stabilized |
| AR-30                    | 2.00x         | 1.40x         | 0.00x       | 0.60x       | Scatter    |
| Experimental Smart Rifle | 1.25x         | 1.50x         | 0.00x       | 0.20x       | Stabilized |
| Pump-Action*             | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Scatter    |
| Hemorrhage Shotgun*      | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Scatter    |
| Explosive Shotgun *      | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Scatter    |
| Choke Shotgun*           | 0.00x*        | 0.00x*        | 0.00x*      | 0.00x*      | Hybrid     |
| Heavy Revolver           | 1.00x         | 1.50x         | 0.00x       | 0.30x       | Stabilized |
| LMG                      | 2.00x         | 1.60x         | 0.00x       | 1.00x       | Scatter    |
| Reserve HMG              | 3.00x         | 2.40x         | 0.00x       | 1.50x       | Scatter    |
| Explosive Cannon         | 0.50x         | 0.70x         | 0.10x       | 0.30x       | Hybrid     |
| Hemorrhage HEL           | 1.70x         | 2.20x         | 0.00x       | 0.10x       | Stabilized |
| Bolt Pistol              | 2.00x         | 2.50x         | 0.00x       | 0.15x       | Stabilized |
| Tracker Rifle            | 2.50x         | 5.00x         | 0.00x       | 0.00x       | Stabilized |
| Sniper Rifle             | 1.00x         | 10.00x        | 0.00x       | 0.00x       | Stabilized |
| Nano Gauss Rifle         | 2.00x         | 7.50x         | 0.00x       | 0.00x       | Stabilized |
* *Shotguns do not use regular spread, they use `Shotgun Cone Size` and `Shotgun Bullet Spread`

### Weapon Changes(Gear Parts):
* Added `O9 Custom GearPart` mod by Ound9
* Added `DS2 Custom Gear Parts` mod by DarkEmperor
* Changed/Added/Removed Gear Parts for some of the guns.

* Hemostasis Medic Gun:
    * Changed `Front Part` to resemble a "sniper rifle" inspired by a certain female egyptian sniper
    * Changed `Sight Part`
    * Changed `Magazine Part`
    * Changed `Receiver Part`
* Heavy SMG:
    * Changed `Front Part`
    * Changed `Receiver Part`
    * Changed `Magazine Part`
    * Changed `Sight Part` 
* Pump-Action Shotgun:
    * Changed `Receiver Part`
* Hemorrhage Shotgun:
    * Changed `Receiver Part`
    * Changed `Magazine Part`
    * Changed `Stock Part` 
* Experimental Smart Rifle:
    * Changed `Front Part`
    * Changed `Receiver Part`
    * Changed `Magazine Part`
    * Changed `Stock Part`
* Explosive Shotgun:
    * Changed `Front Part`
    * Changed `Receiver Part`
    * Changed `Sight Part`
    * Changed `Stock Part`
* Heavy Revolver:
    * Changed `Front Part` to have a `scope`
    * Changed `Stock Part`
* LMG:
    * Changed `Magazine Part`
* Reserve HMG:
    * Changed `Front Part` into a `Minigun` (Yes I know it's not )
    * Changed `Stock Part`
    * Changed `Receiver Part`
* Explosive Cannon:
    * Changed `Front Part` to look like a grenade launcher
    * Removed `Magazine Part`
    * Changed `Receiver Part`
    * Removed `Sight Part`
* Hemorrhage HEL:
    * Changed `Front Part`
    * Changed `Receiver Part`
    * Changed `Magazine Part`
    * Changed `Sight Part`
* Bolt Pistol:
    * Changed `Front Part`
* Sniper Rifle:
    * Changed the `Scope Part` to also have a `thermal attachment` as well as a `scope`
* Nano Gauss Rifle:
    * Changed the `Front Part` to resemble a `Railgun`
    * Changed `Scope Part`
    * Changed `Receiver Part`
    * Changed `Stock Part`
    * Removed `Magazine Part`
* HMG Turret:
    * Changed `Front Part`
    * Changed `Receiver Part`
* Shotgun Turret:
    * Changed `Front Part`

### Weapon Tweaks:
* Properly rearranged weapon's list based on alphabetical order.
* Updated `ExtraWeaponCustomization` mod to v3.7.11
* Bots and Turrets can now utilize most of EWC's custom properties. For example explosive, biotag, projectile(not recommended, they will miss a lot), and etc.
* Switched `WeaponStatShower` mod by DacreDOLOLO to `DescriptiveWeaponStatShower` by Amorously.
    * Feel free to remove the WeaponStatShower mod from the list. It will still be fine to have both, but the newer version will be loaded instead of the original mod.
* Added a brief description for all guns with traits.
* Added sound effects for some weapons with missing and awkward animations.
* Added `AmorLib` mod by Amorously. A new dependency for EWC with v3.7.11 update.
* Fixed some weapons with incorrect sub-names such as `Thermal Subgun` to `Thermal Bio-Tag Subgun`
* Hemostasis Medic Gun:
    * Increased Direct Damage from `0.1` to `1.0`
* Nano Foam Pistol:
    * Increased Direct Damage from `0.1` to `1.0`
    * Increased Armor Shred debuff from `20%` to `30%`
    * Decreased Armor Shred cap from `40%` to `30%`
    * Increased duration of both Armor Shred and Foam from `5.0s` to `6.0s`
    * Added sound effect once the magazine reaches 6.0; even while holstered. 
* HEL Revolver: **Rework**
    * Decreased Direct Damage from `13.6` to `5.0`
    * Increased Precision Multiplier from `0.9x` to `4.2x`
    * Decreased Max Ammo Capacity from `128` to `116`
    * Decreased Reload time from `2.2s` to `2.1s`
* Heavy Revolver: **Rework**
    * Renamed from `Bataldo Heavy Revolver` to `Van Auken Heavy Revolver`
    * Decreased Direct Damage from `35.9` to `10.0`
    * Increased Precision Multiplier from `0.95x` to `6.2x`
    * Decreased Max Ammo Capacity from `118` to `106`
    * Decreased Reload time from `2.15s` to `2.1s`
* 5-B Bullpup:
    * Increased Max Ammo Capacity from `442` to `508`
* Tracker PDW:
    * Increased Direct Damage from `3.0` to `3.2`
    * Increased Magazine Size from `20` to `22`
    * Decreased Max Ammo Capacity from `412` to `388`
* Heavy SMG:
    * Increased Shot Delay from `0.12s` to `0.20s`
    * Increased Direct Damage from `5.7` to `6.0`
    * Decreased Max Ammo Capacity from `391` to `379`
* 3-B Carbine:
    * Increased Direct Damage from `3.3` to `3.4`
* Single Slug Shotgun:
    * Decreased Direct Damage from `55.6` to `55.0`
    * Increased Max Ammo Capacity from `51` to `60`
    * Increased Reload Time from `1.3s` to `2.0s`
    * Added `Reload Speed` modifier on Kill
        * Any enemy kill with the slugger will lower the reload time from `2.0s` to `1.0s` for a short duration
        * The buff duration is `2.5s`
* Heavy Rifle:
    * Increased Max Ammo Capacity from `434` to `452`
* Medic Gun:
    * Increased Healing from `0.5%` to `0.62%` per tick
* Assault Rifle:
    * Increased Direct Damage from `6.9` to `8.1`
    * Decreased Magazine Size from `25` to `20`
    * Decreased Max Ammo Capacity from `221` to `203`
    * Increased Shot Delay from `0.16s` to `0.3s`
* AR-30:
    * Decreased Direct Damage from `7.0` to `6.5`
    * Increased Max Ammo Capacity from `255` to `305`
    * Decreased Reload Time from `1.8s` to `1.7s`
* Exp. Smart Rifle:
    * Added sound effect to the Lock-on System
* Explosive Rifle:
    * Decreased Explosion Damage from `15.0` to `11.0`
    * Increased Direct Damage from `8.5` to `15.5`
    * Decreased Max Ammo Capacity from `80` to `72`
* Explosive Cannon:
    * Increased Direct Damage from `5.9` to `3.1`
    * Increased Magazine Size from `5` to `6`
    * Decreased Max Ammo Capacity from `50` to `42`
    * Increased Reload Time from `4.0s` to `4.5s`
    * Increased Equip Time from `0.8s` to `1.0s`
    * Added `Hold Aim to Rapid Fire` property
* Choke Mod Shotgun:
    * Increased Direct Damage from `6.4` to `8.8`
    * Increased Magazine Size from `4` to `5`
    * Increased Max Ammo Capacity from `54` to `60`
    * Decreased Pellet Count from `8` to `5`
* Pump-Action Shotgun:
    * Decreased Reload Time from `3.0s` to `2.5s`
* Hemorrhage Shotgun:
    * Decreased Shotgun Cone Size from `2` to `4`
    * Increased Shotgun Bullet Spread from `2` to `4`
    * Increased Shotgun Bullet Count from `8` to `10`
* Hemorrhage HEL:
    * Increased Damage Over Time Bleed from `19.0` to `25.0`
    * Decrease Charge Up Time from `0.25s` to `0.2s`
    * Added `Auto Aim` Property only while Aiming.
* LMG:
    * Added Bullet Pierce Limit of `+1`
    * Increased Magazine Size from `60` to `70`
    * Increased Max Ammo Capacity from `360` to `413`
* Reserve HMG:
    * Added Bullet Pierce Limit of `+1`
    * Decreased Charge Up Time from `0.6s` to `0.5s`
    * Increased Shot Delay from `0.08s` to `0.2s`
    * Increased Max Ammo Capacity from `742` to `885`
    * Added `Accelerate` property.
        * HMG will fire significantly faster the longer you hold the trigger.
    * Added `Recoil` property.
        * Decreased the overall recoil of the gun since it is insanely high and impossible to control.
* Nano-Gauss Rifle:
    * Increased Direct Damage from `40.3` to `50.5`
    * Increased Magazine Size from `4` to `5`
    * Decreased Reload Time from `3.5s` to `3.0s`
    * Changed from `Hitscan` to `Projectile`

### Tool Tweaks:
* Sniper Sentry:
    * Increased Shot Delay from `2.1s` to `2.5s`
    * Decreased Effective Range from `70.0m` to `60.0m`
* Burst Sentry:
    * Increased Direct Damage from `4.5` to `4.6`
    * Increased Burst Shot Count from `3` to `4`
    * Increased Burst Shot Delay from `1.0s` to `2.0s`
    * Increased Effective Range from `20.0m` to `30.0m`
* Machine Gun Sentry:
    * Increased Stagger Multiplier from `2.5x` to `3.0x`
    * Decreased Spread Fire from `2.0x` to `1.5x`
    * Decreased Direct Damage from `1.7` to `1.6`
    * Increased Shot Delay from `0.8s` to `1.0s`
    * Increased Pierce Limit from `1` to `2`
    * Increased Max Ammo Capacity from `1096` to `1594`
    * Added `Ammo Usage` property of `-1`
    * Added `Multishot` property of `+1`. Fires a second bullet for double damage, but wastes ammo twice as fast!
    * Increased Effective Range from `10.0m` to `15.0m`
* Shotgun Sentry:
    * Increased Shot Delay from `1.25s` to `1.3s`
    * Increased Pierce Limit from `0` to `1`
    * Increased Effective Range from `5.0m` to `7.5m`

### Melee Tweaks:
* Sledgehammer:
    * Decreased Max Charge Time for Heavy Attack from `3.5s` to `3.0s`
* Spear:
    * Decreased Max Charge Time for Heavy Attack from `4.2s` to `3.7s`
* Bat:
    * Increased Max Charge Time for Heavy Attack from `1.5s` to `2.0s`
    * Fixed explosive kills triggering by any death from original explosion. Now the Explosion will only occur by the player's kill.

### Player Tweaks:
* Decreased the `AmmoStandardInitial` & `AmmoSpecialInitial` from `300` to `250` (Starting Ammo for Main and Special weapon slots)
* Increased the `ResourcePackMaxCap` from `400` to `500`
    * Old:
        * 13% = 94 HMG
        * 14% = 200 MP1
    * New(w/3 booster):
        * 16%(21%) = 117(154) HMG
        * 17%(23%) = 250(330) MP1
    * Quartermaster(w/3 booster): Keep note that classes with higher or lower Ammo/Tool cost efficiency will have different supply values.
        * 21%(26%) = 198(247) HMG
        * 23%(28%) = 426(531) MP1

### Class Tweaks:
* All Classes(except Shock Trooper, Demolitionist, Deprived, Courier)
    * Decreased Baseline Explosive Resistance by `-20%`

* Marine:
    * Increased Bleed Resistance bonus from `+50%` to `+70%`
    * Increased Melee Armor & Damage penalty from `-40%` to `-50%`

* Shock Trooper:
    * Increased Max Health bonus from `+20%` to `+30%`
    * Added Explosive Resistance of `+30%`
    * Added Bio Scan Speed penalty of `-20%`

* Quartermaster:
    * Increased Regen Cap bonus from `+55%` to `65%`

* Specialist:
    * Decreased Bioscan Spd. & Scanner Recharge from `+50%` to `+30%`

* Field Technician:
    * Decreased Sentry CPUs from `+40%` to `+30%`

* HEL Diver:
    * Increased HEL Damage bonus from `+75%` to `+100%`
    * Increased Bullet Resistance penalty from `-25%` to `-50%`

* Abhuman:
    * Increased Melee Hitbox & Range bonus from `+25%` to `+40%`

### Booster Tweaks:
* Increased Muted/Bold/Aggressive `Revive Health` booster by flat `5%`(total potential value from `30%` to `45%`)

### Syringe Tweaks:
* Virus Bomb Syringe:
    * Increased Damage from `300` to `350`
    * Increased Range from `5.0m` to `7.5m`
    * Increased Infection from `15%` to `25%`

* Virus Nuke Syringe:
    * Increased Damage from `600` to `700`
    * Increased Range from `7.5m` to `15.0m`
    * Increased Infection from `25%` to `50%`

### QoL Additions:

* Added `ChatterReborn` mod by *easternunit100*
* Added `DropItemFixed` mod by *Dinorush*
* Added `BetterBots` mod by *easternunit100*

---

* Note: To find patch notes before v2.0, please check the Github repo.
