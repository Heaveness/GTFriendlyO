# Changelog

## **v2.0.6** - Latest

### Emergency Hotfix:

* Fixed some changes not included in v2.0.5 by accident.
> Dev Note: Apologies, I accidentally uploaded the wrong changes into v2.0.5

---

### v2.0.5

### Mod Additions:
* Added `SpreadStartingAmmo` mod by Dinorush
* Ammo is spread from a pool given to players on startup based on how many players are present. If a player/bot joins then the pool is reduced to accommodate the new player(s), dismissing the slot will not refund the lost ammo from the distribution.
    * 1 Player: 4x ammo
    * 2 Players: 2x ammo 
    * 3 Players: 1.33x ammo
    * 4 Players: 1x ammo (Bots count as players)
> Dev Note: Originally this was added in accidentally in v2.0.2, but after a second(& third) opinion on it. I was told I was overthinking the issue and in long-term should balance the game for smaller lobbies. This should make solos, duos, and trios have more enjoyable time. Since my modpack was forcing 3-4 player lobbies in the later rundowns.
* Updated `BetterBots` mod

### Weapon Fixes & Tweaks:
* Bolt Pistol:
    * Increased Precision Multiplier from `0.6x` to `0.7x`
    * Increased Stagger Multiplier from `1.5x` to `2.0x`
> Dev Note: Previously the Bolt Pistol was able to one shot a scout reliably, but the recent changes on precision and stagger has unintentionally made it awkward. It should be possible to one shot scouts properly at any direction.
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
> Dev Note: Fixed an issue where the Sniper Rifles has trouble killing Giants since their increased base health. A sniper rifle should feel powerful in the right hands.
* Reserve HMG:
    * Increased Stagger Multiplier from `1.8x` to `2.0x`
    * Once again trying to fix this gun's first person model after fixing the third person model from a previous patch.
> Dev Note: Getting sick and tired of trying to fix this gun... Alright, if it doesn't get fixed by this patch then I am going to just move on. I am losing time over this pointless bug.

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
> Dev Note: Fixed the awkward shooting of the burst and shotgun turrets that made it very jarring to use in close-mid range engagements. I may have overdone the shot delay, apologies on my part.

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
> Dev Note: After some feedback and playtesting, I found them to have lost a lot of their strength. They struggle to kill even the lower tier enemies.

### Enemy Fixes & Tweaks:
* Added underline text for all tagged enemies to help separate the name and healthbar for visual clarity.
* Shadows:
    * Fixed this variant not creating infected fog spheres on death when hibernating.
* Striker Giants:
    * Increased Body Part Health from `300` to `450`
    * Increased Weakspot Damage Multiplier from `0.4x` to `0.6x`
> Dev Note: Still wasn't enough to make precision weapons rewarding against these targets. Now their head should be same health as their baseline health. As well as high-cal sniper should be able to kill Giants in one shot to the head.

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
> Dev Note: Originally it was applying the wrong amount of armor shred which was giving a tiny buff that was negligible at best. It should properly apply the right amount.
* Medic Gun:
    * Added `Ammo Mod` property
    * Killing an enemy with the venom darts will restore `1.0` ammo back into the reserve.
        * Does **NOT** refund more than 1 dart per kill.
> Dev Note: While the medic gun should primarily be used to heal teammates. And the venom darts on only enemies. Unfortunately, the low ammo efficiency and low overall damage made players only save it for larger targets for its silence debuff. Effectively making the gun undesirable in many horde situations. With this change you will receive 1.0 ammo back after a kill(it will NOT refund more than 1, even if you use more than 2 darts to kill). Which often only happens on smaller targets, so it's not as punishing.
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
> Dev Note: I have completely forgotten to change the ricochet bullet's stats to the current base gun's values. It still had the old stats which unintentionally made it too strong. Other the side note, the ricochet aspect created bad habits out of the player. There was little to no punishment for simply firing wildly. The gun should still be fun enough on its own, but it's not as abuseable as before.

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
> Dev Note: This slight rework was to make sledgehammers differ a bit from the Spear's flat armor pierce. Instead I gave the sledgehammer a party buff by making the target take more damage from most sources for a short duration.
* Knife:
    * Increased Light Backstab Multiplier from `2.0x` to `2.1x`
    * Increased Heavy Backstab Multiplier from `2.5x` to `2.6x`
    * Decreased Total DoT Damage from `6.0` to `5.0`
    * Decreased stack limit from `unlimited` to `4`
    * Increased DoT timer from `3.0s` to `4.0s` (takes a little longer to reach total damage)
> Dev Note: This is sort of a nerf to the knife's potential damage with infinite bleed stacks. It's a powerful tool that can dominate stealth runs, but the unlimited bleed stacking gave it insane damage potential with the right methods. I just want to prevent cheesing without decreasing its stealth capabilities. 
* Spear:
    * Removed can hit multiple targets, unintentional.
    * Increased Armor Pierce bonus from `+10%` to `+15%`
> Dev Note: Spears piercing multiple targets never worked properly and it was awkward to capitalize; served no real purpose.
* Bat:
    * Decreased Explosion Damage from `10.0` to `5.0`
    * Increased Explosion Stagger Multiplier from `1.5x` to `3.5x`
> Dev Note: Lowered the explosion damage but increased the stagger damage potential since this weapon has always been a crowd control melee option.

---

### v2.0.3

* Dev Note: If you have any feedback on the modpack, please do not hesitate to comment in the github issue tab [here](https://github.com/Heaveness/GTFriendlyO/issues)!

### Mod Updates:
* Updated `ExtraWeaponCustomization` mod.
* Updated `GTFuckingXP` mod.
* Removed `SpreadStartingAmmo` mod <= **IMPORTANT**
> Dev Note: the SpreadStartingAmmo mod was an accidentally addition to the mod pack. I apologize for its inclusion, it was not my intention to add this one. If you already have it installed, please REMOVE it as it breaks balancing.

### Enemy Tweaks:
* Striker Giant:
    * Increased Body Part Health from `200` to `300`
> Dev Note: This is to prevent the weakspot part(head) from breaking too soon against high-powered weapons. Their overall health did not increase from this change. It just means the sniper rifle can consistently kill Giants with two shots to the head without worrying about the head breaking.

### Weapon Fixes:
* Reserve HMG:
    * Fixed third person model of the gun being upside down.
> Dev Note: I think I have found the main culprit of this problem. It should be fixed now.
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
> Dev Note: This was a mistake by lowering the MP1's stagger power. This change with its base damage has unintentional made this gun significantly worse by accident. My apologies on that oversight.

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
> Dev Note: Fixed some inconsistency in the descriptions. Numbers will be given in the wiki page, not in-game as it clutters the space. Sadly, the game automatically shrinks the text size if there is too much.
* Fixed typos in README file
* Fixed typos in CHANGELOG file
> Dev Note: Been awhile, whoops! ~(ツ)~

---

### v2.0.1
> Dev Note: This patch is to fix some of the issues arised from the previous update. As well as improving on other aspects that was missed/ignored with that update.

### Class Tweaks:
* Courier:
    * Increased Infection/Explosion/Bullet/Bleed Res. penalty from `70%` to `80%`
    * Removed Initial Tool Ammo bonus.
> Dev Note: I have received some feedback regarding the Courier class being very fun, which is good. But also on it being too strong. The Living Bio Tracker ability is extremely powerful tool which I cannot adjust directly. So I have bring the class down a bit, but not too much. I still want people to enjoy playing this class. This is a meme class so balance isn't its main focus, but I know when a class is a bit too powerful that it can overshadow others.
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
> Dev Note: Scouts should be less frustrating to deal with in specific rundowns where multiple are present in a room. With these new changes, players can just barely move out of the way of their feelers; even while at baseline crouching speed. Classes with faster movement speed will have much easier time; especially the Covert Op class. The increased tentacle count will often be shot downwards by their AI, which prevents players from being too close prematurely. Timing is key.

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
> Dev Note: Main reason for this change is because the original HEL shotgun was not using the HEL booster effect. Unfortuntely, this makes this gun redundant as another gun fills a similar role. 
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
> Dev Note: I am aware there is a third-person model issue with this gun. It is being held upside down, unfortunately I have tried numerous methods to no avail. I will give up on it otherwise this update will never come out. I will look into a fix in the future, if I feel like it.
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
> Dev Note: These two melee weapons should feel less clunkier to use. This is additional decrease from the last patch.

### Player Tweaks:
* Increased the `AmmoStandardInitial` & `AmmoSpecialInitial` from `250` to `275` (Starting Ammo for Main and Special weapon slots)
> Dev Note: I might have nerfed this aspect a bit too harshly from the previous update.

### Misc.
* Updated `ExtraWeaponCustomization` mod
* Updated `MovementSpeedAPI` mod
* Updated `ExtraEnemyCustomization` mod
* Updated `ExtraSyringeCustomization` mod

---

### v2.0.0 Final Major Update

### Weapon Rework(Precision & Stagger Multiplier):
* The vanilla GTFO baseline precision is 0.74x because it is added on top of enemy's weakspot multipliers. Each enemy has their own weakspot multiplier which I will not provide here, they haven't changed from vanilla values.
> Dev Note: This will however might change how some weapons will feel overall.  Many of these values were left mostly untouched as I did not know how to properly calculate the damage numbers. After some research, I was able to figure out a decent middle ground between precision and stagger. As a result, some guns might feel stronger or weaker after this update but I believe it's important for the pack's overall health.

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
> Dev Note: The values here was mainly done through feeling alone. After figuring out a more consistent and better method, I decided to rebalance the nature of damage falloffs.

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
> Dev Note: This update has massively increased in scope in the last two weeks. The goal is to finalize the overall feeling of all the guns for this final major update. Hipfire spread exists to simulate difficulty making accurate shots based on the gun's muzzle "climb"(other than recoil) and Aimed spread was to show off "bracing" the gun to make better controlled shots. But I noticed all guns especially spray like LMGs and Shotguns have 100% accuracy while aiming. This can cause some guns feel more like a different version of another gun, which can make some classes feel less impactful and unique to their identity. So these changes are made to help simulate the difference between a precision(Stabilized) and spray(Scatter) weapon.

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
> Dev Note: Not a fan of how some guns did not have good scopes or the overall design of a few guns didn't match with their custom weapon properties. Some guns looked like clones of other firearms, so this should give them a new fresh coat of paint.

* Hemostasis Medic Gun:
    * Changed `Front Part` to resemble a "sniper rifle" inspired by a certain female egyptian sniper
    * Changed `Sight Part`
    * Changed `Magazine Part`
    * Changed `Receiver Part`
> Dev Note: Yes, I know it doesn't look like a SMG anymore. Techman Biotechnics is a weird manufacturing company.
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
> Dev Note: The main reason for the both medic gun and foam pistol direct damage tweaks is to scale with new Stagger Multiplier changes.
* Nano Foam Pistol:
    * Increased Direct Damage from `0.1` to `1.0`
    * Increased Armor Shred debuff from `20%` to `30%`
    * Decreased Armor Shred cap from `40%` to `30%`
    * Increased duration of both Armor Shred and Foam from `5.0s` to `6.0s`
    * Added sound effect once the magazine reaches 6.0; even while holstered. 
> Dev Note: Foam Pistol should have overall better feeling during combat. Now players requires only one shot to maximize the armor shred potential.
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
> Dev Note: I want revolvers to have a more unique identity to the other sidearms by having it rely on precision shots to do actual damage while body shots are heavily discouraged. Ricochet bullets will automatically try to hit weakspots than any other body parts.
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
> Dev Note: Makes the slugger a more interesting weapon. The higher base reload time will incentize players to make accurate shots. Then getting kills will reward the player with a faster reload buff.
* Heavy Rifle:
    * Increased Max Ammo Capacity from `434` to `452`
* Medic Gun:
    * Increased Healing from `0.5%` to `0.62%` per tick
> Dev Note: This is to compensate from the previous patch that increased Medic Gun's damage to 1.0. This change accidentally made them hurt the players more too. As a certain wise medic once said "If you do it wrong, it's going to hurt. If you do it right, it's going to hurt a lot."
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
> Dev Note: Changed Explosive Cannon to have a stronger identity to the Explosive Rifle and Shotgun. It will feel more like a traditional grenade launcher.
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
> Dev Note: The LMG and HMG should be feel more useful to utilize against crowds. The new HMG is a lot of fun!
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
> Dev Note: With the recent patches that buffed turrets and Field Technicians, they are incredibly powerful. So I realized that increasing the delays between the shots will prevent some hard scaling. I will look closely to make adjustments where needed.

### Melee Tweaks:
* Sledgehammer:
    * Decreased Max Charge Time for Heavy Attack from `3.5s` to `3.0s`
* Spear:
    * Decreased Max Charge Time for Heavy Attack from `4.2s` to `3.7s`
* Bat:
    * Increased Max Charge Time for Heavy Attack from `1.5s` to `2.0s`
    * Fixed explosive kills triggering by any death from original explosion. Now the Explosion will only occur by the player's kill.
> Dev Note: I am trying to make Sledgehammer and Spear be a little less clunky when charging for a Heavy. Bat is very strong, so I am only making their heavy swing take longer to charge.

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
> Dev Note: This change was to elevate potential issues with the new unified ammo reserves from a previous patch. Some guns simply became difficulty to maintain and was forced to use melee. While I believe players being forced to use melee when little or no ammo is fine as it increases the tension and challenge. I also believe that being constantly forced to melee will only hurt the enjoyment of pure ranged classes. So a player or class that really specializes on Supply Pack Efficiency should feel more impactful, but the baseline increase should prevent it from being 100% necessary(especially in some missions). Hopefully, this will give players a bit more freedom to choose.

### Class Tweaks:
* All Classes(except Shock Trooper, Demolitionist, Deprived, Courier)
    * Decreased Baseline Explosive Resistance by `-20%`
> Dev Note: I'm not a fan of just nerfing explosive weapons' numbers because they should be fun to use. But I also believe that they are on the over-performing side. So the changes should affect more in the player's decision making. That's why they should have a higher chance of killing your teammates!

* Marine:
    * Increased Bleed Resistance bonus from `+50%` to `+70%`
    * Increased Melee Armor & Damage penalty from `-40%` to `-50%`

* Shock Trooper:
    * Increased Max Health bonus from `+20%` to `+30%`
    * Added Explosive Resistance of `+30%`
    * Added Bio Scan Speed penalty of `-20%`
> Dev Note: While I'm not a fan of nerfing a class. Unfortunately, the Shock Trooper has a lot of versatility with shotgun choices and great stat bonuses. Their only "real" penalty is the negative movement speed if they ignore the other weapons. So this change is to incentivize the class to move out of bioscans to rush towards enemies instead of hanging back for objectives. Also the explosion resistance will punish Shock Troopers less if there is a Demolitionist in the team. This does mean that any full-team scans will take 20% longer with this class, which can be countered if paired with the Specialist class or boosters. So weigh your options with the team.

* Quartermaster:
    * Increased Regen Cap bonus from `+55%` to `65%`
> Dev Note: The class needed a bit more health regen cap to reach roughly 49% - 50% baseline cap; It's occasionally off by a few percent what with free will and all.

* Specialist:
    * Decreased Bioscan Spd. & Scanner Recharge from `+50%` to `+30%`
> Dev Note: This is a very powerful booster effect, which can trivialize some of the bio scan objectives on certain missions. It should have some level of synergy/counter with the Shock Trooper if both classes are in the same lobby.

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
> Dev Note: These syringes were designed as last-resort crowd clearers with a heavy infection penalty. However, players might notice that infection resistance can be negated with enough resistance stat booster. In particular, a particular support class(Paramedic) may find themselves uniquely suited for a high-risk high-reward detonation plan. Although, use it with utmost care as it can easily kill your living teammates too.

### QoL Additions:

* Added `ChatterReborn` mod by *easternunit100*
> Dev Note: Makes communication easier between players without having to always use voice chat to relay all of the information. The characters themselves should be doing some of the lifting.
* Added `DropItemFixed` mod by *Dinorush*
> Dev Note: This is to make the inventory management feel less of a hassle. Often players would have to play a weird game of picking up different items just to trade with another player.
* Added `BetterBots` mod by *easternunit100*
> Dev Note: This is probably the most controversal addition on this list, but EWC(Extra Weapon Customization) mod works with bots now. This is improve their AI so they don't get stuck on certain terrain especially during scans. It will also prevent them from opening containers themselves which will cause them to grab an item immediately. They will only grab if the player opens them first. Be warned... do **NOT** give bots `explosive` weapons.

---

### v1.4.2

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

---

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
* Increased Damage for Virus Bomb Syringe from `250` to `300`
* Increased Damage for Virus Nuke Syringe from `500` to `600`
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