# Changelog

## **v2.4.0** - Latest

### Personal Note:
* It's generally fine to update any mods. Regular bug fixes and QoL improvements are always welcome, but be cautious when updating mods with large changes. Keep in mind that every mod update has the potential to break something within this pack. Even I cannot guarantee every update stability. So you should personally do your research before updating them.

* With the addition of keybind-based triggers that came along with `v2.3.0`. **PLEASE** check the EWC(ExtraWeaponCustomization) config and change the keybind to **YOUR** settings. I am aware that not everyone have keypads for their setup. 
    * Go to `Edit Config` within Thunderstore client -> Search for `ExtraWeaponCustomization.cfg` -> `Edit Config` -> Change keybinds 1 through 4 under `Keybind Settings` section
    * Be advised that any keybind changes might reset with each update.

* Please let me know on my [Github](https://github.com/Heaveness/GTFriendlyO/issues) issue page if there are problems or if you have feedback check this [Github](https://github.com/Heaveness/GTFriendlyO/discussions) discussion page. Thanks and have fun! 

### Mod Updates:
* Updated `ModifierAPI` mod
* Updated `Informative Door Icons` mod
* Updated `EEC H` mod
* Updated `Spectate` mod
    * Added `Clonesoft Json` dependency mod by AuriRex
    * Added `PlayerSync` dependency mod by food
* Updated `GTFuckingXP` mod
    * Shows player class underneath their name during rundown
    * Shows currently selected class on the class selector button
* Updated `Minimap` mod
    * Minimap should properly disable during EMP events
* Added `YeetArtifactHeat` mod by JarheadHME
    * Removes the text of GTFO Heat since Artifacts aren't a thing in this modpack
    * End screen still says something about it, can't fix it for now
* Added `Tweaker` mod by Dex
* Added `Slides Bot Control` mod by Slide
    * Gives players the ability to give commands to bots through a radial menu(Default Key: X) or Smart Select(Default Key: V).
    * Significant improvement to lobbies that don't have a full group to play.

### Object Carry Rework:
* Removed `StrongerPrisoner` mod
    * It is safe to remove this mod from your list. I highly recommend it.
> Dev Note: This mod was removed because it has made some objectives significantly easier, especially with specific classes. But I also understand how annoying certain items felt like a slog to carry throughout a level.
* Added `Heavyweight` or `Lightweight` to all weapon trait descriptions
* Can/Cannot Sprint While Holding:
| Item/Gear Changed		| Sprint? |
|:----------------------|:-------:|
| Battery Cell 			| Yes 	  |
| Fog Turbine 	       	| Yes  	  |
| Objective Items       | No      |
| Javelin Rifle 	    | No      |
| Explosive Rifle     	| No 	  |
| Arc Subjugator     	| No 	  |
| LMG               	| No 	  |
| Reserve HMG(Minigun) 	| No      |
| Exp. Smart Rifle      | No      |
| Nano Gauss Rifle   	| No      |
| Wisp Launcher		    | No      |
| Sniper Rifle 		    | No      |
| Flamer Tool	       	| No      |
| RYN0 Annihilator    	| No      |
| Sentry Turrets   	    | No      |
> Dev Note: Main reason for these changes is to give these weapons/tools some weight. It's to provide more identity to both heavier and lighter weapons/tools in your arsenal. As carrying an entire loadout of heavy-duty powerful weapons should effectively slow the player down. While those that want a light loadout should be able to be nimble.

### Player Tweaks:
* Tweaker Mod:
    * Increased Baseline Sliding Distance from `1.0m` to `4.0m` (slide further; affected by friction/obstacles and other movement speed modifiers)

### Weapon & Tool Tweaks:
* Updated `DescriptiveWeaponStatShower` mod
    * All weapon descriptions and stats in the loadout selection can be switched by clicking on the box or number arrows
    * All trait descriptions has been reworded.

* DMR: **Rework**
    * Combined `DMR` and `Double Tap Rifle`
        * Their respective base stats will stay the same when switching modes
    * Increased Max Ammo from `187` to `220`
    * Increased Clip Size from `10` to `20`
    * Increased Reload Time from `2.3s` to `2.5s`
    * Switch between `2` modes(Semi-Auto & 2-Burst Fire):
        * Semi-Auto:
            * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
            * Increased Precision Multiplier from `1.0x` to `1.15x`
        * 2-Burst Fire:
            * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])
            * Increased Stagger Multiplier from `1.4x` to `1.6x`
> Dev Note: Both weapons basically filled the exact same role with similar results, but the method was done differently. So I believed it was a healthier choice to combine the two to allow for more gameplay options.

* Double Tap Rifle: **Removed**
    * Combined `DMR` and `Double Tap Rifle` (read above)

* Triple Barrel:
    * Slight improvement to trait description

* Beam Rifle:
    * Slight improvement to trait description
    * Increased Shot Delay from `0.02` to `0.05`
    * Decreased Projectile Hit Size Bonus from `+0.5m` to `+0.3m`
    * Added `Movement Speed` Property during firing:
        * Decreases User's movement speed by `-70%`
        * Duration: `Start to End Firing`
> Dev Note: I am hoping this will increase the game's performance a bit during multiplayer lobbies. The movement speed penalty has two purposes: first to incentize better positioning, and second its to prevent weird interactions with the beam with fast movement speed.

* Exp. Smart Rifle:
    * Changed Locked Target color to `Green`

* Bat:
    * Increased Explosion Radius from `2.5m` to `3.0m`
    * Increased Explosion Stagger Multiplier from `3.5x` to `8.0x`

* Medic Gun:
    * Increased Mode 1's DoT Total Damage from `25.0` to `30.0`
    * Increased Mode 2's DoT Total Damage from `1.0` to `2.0`
    * Changed Mode 2's DoT Damage Distribution from `End` to `Uniform`
    * Increased Mode 2's Stagger Multiplier from `40.0x` to `80.0x`
    * Increased Mode 3's Armor Buff from `+20%` to `+25%`
    * Increased Mode 3's Armor Shred from `-30%` to `-40%`
> Dev Note: Incentize players to use its offensive capabilities as a viable option.

* Heavy SMG:
    * Increased Max Ammo from `379` to `391`
    * Increased Stagger Multiplier from `1.2x` to `1.3x`
    * Decreased Hipfire Spread from `2.3x` to `2.0x`
    * Decreased Aimfire Spread from `0.3x` to `0.15x`

* C-Foam Launcher:
    * Decreased Max Charge Timer from `2.5s` to `2.0s`

* Explosive Mine Deployer:
    * Increased Placement Range from `6.0m` to `8.0m`

* Foam Mine Deployer:
    * Increased Placement Range from `6.0m` to `12.0m`
    * Increased Foam Bubble Count from `25` to `30`
    * Increased Bubble Angle from `14` to `45`
    * Increased Bubble Minimum Speed from `7` to `10`
    * Increased Bubble Maximum Speed from `13` to `15`

* Consumable Foam Mine:
    * Increased Foam Bubble Count from `14` to `18`
    * Increased Bubble Angle from `14` to `16`

* Exterminatus Flamer:
    * Increased DoT Stack Size from `10` to `20`
    * Increased Stagger Multiplier from `1.0x` to `1.5x`
> Dev Note: Should be a bit more effective against larger targets. That also includes teammates...

* RYN0:
    * Increased Minimum Explosion Damage from `400.0` to `500.0`
    * Increased Maximum Explosion Damage from `800.0` to `1000.0`
    * Decreased Friendly Fire Modifier from `0.1x` to `0.07x`
> Dev Note: Because why not? It's extremely expensive and risky weapon to utilize. So might as well make sure most things die from a single shot.

* Missile Turret:
    * Increased Explosion Damage from `40.0` to `50.0`
    * Increased Shot Delay from `4.5s` to `5.0s`

* Sniper Turret:
    * Changed `Front` Gear Part

### New Weapon:
* Hanaway Javelin Rifle:
    * Created in cooperation between Hanaway Precision Systems and Omneco Networks
    * Fires fast projectiles that stick onto targets
    * Thermal-Assist Scope only when aiming
    * Activate with keybind or reload to "electrocute" hit targets, explodes on electrocution kill.
        * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
        * Direct Damage: `10.0`
        * Clip Size: `5`
        * Max Ammo: `40`
        * Reload Timer: `4.5s`
        * Activation Delay: `0.5s`
        * Total DoT: `55.0`
        * DoT Duration: `4.5s`
        * Tick Rate: `6.0`
        * Stack Limit: `5`
        * Precision Multiplier: `1.0x`
        * Stagger Multiplier: `100.0x`
        * Friendly Fire Multiplier: `0.2x`
        * Explosion Damage: `5.0`
        * Explosion Radius: `6.0m`
        * Explosion Stagger Multiplier: `2.0x`
        * Push based on shooting during standing/crouching/jumping:
            * Standing: `-4.0m`
            * Crouching: `-1.0m`
            * Jumping: `-6.0m`
> Dev Note: Replaces the removed Double Tap Rifle. This gun has great damage and crown control for larger enemies. But its low ammo and high base damage is overkill against smaller targets.

* Omneco Arc Subjugator:
    * Requires a lock-on to fire.
    * Fires a "harpoon" at a target that will also chain to another nearby target. Prioritizes highest health enemies.
    * Immediately electrocutes both targets with very high stagger damage.
    * Applies Increased Damage Debuff, Silence CC, and BioTag onto targets for the duration.
    * Significantly decreases player's movement speed, but increases damage resistance during DoT duration.
    * Requires manual charging(reload) `4` times to fire the gun.
    * Infinite Ammo
    * Cannot switch gear or reload during the electrocution duration.
        * Direct Damage: `1.0`
        * Shrapnel Count: `1` after first bullet hit
        * Ballistic Type: `Slow Projectile`
        * Max Ammo: `Infinite`
        * Reload Timer: `2.0s` per manual reload(requires `4` to fire)
        * Electrocution Total Damage: `10.0`
        * Stagger Multiplier: `500.0x`
        * DoT Duration: `25.5s`
        * Bio Ping Duration: `25.5s`
        * Silence CC Duration: `25.5s`
        * Movement Speed Multiplier: `-85%` (Player)
            * Can be resisted through movement speed boosts
        * Damage Resistance: `+20%` (Player)
            * Can stack with other damage resist up to `+40%`
        * Damage Taken Debuff: `+50%` (Enemy)
> Dev Note: This weapon was an idea that I had for a long time since v2.0, but couldn't execute correctly. There wasn't enough properties and features available at the time. This is a pure support weapon that synergizes very well with any team or weapon composition, but has very clear drawbacks.

### New Tool:
* Concussive Nade Turret:
    * Fires Low Damage, High Stagger, & Cluster Grenades.
    * More CC-oriented than lethal damage. Enemies take increased damage taken from all sources during CC.
    * Applies `Silence CC` on hit, disables some abilities like non-boss tongues and Needler projectile barrages, but NOT scout screams or melee attacks.
    * Strong gravity projectiles, requires higher elevation to get the most value.
        * Direct Damage: `1.0`
        * Cluster Bomblet Count: `8`
        * Effective Range: `30.0m`
        * Explosion Damage: `2.0`
        * Explosion Radius: `7.5m`
        * Explosion Stagger Multiplier: `250.0x`
        * Shot Delay: `10.0s`
        * Max Ammo `160`
        * Ballistic Type: `High Gravity Projectile`
        * Effective Range: `30.0m`
        * Explosion will not hurt friendlies, but owner can get hit.
        * Placement Time: `0.6s`
        * Pickup Time: `1.0s`
        * Deploy Time: `3.0s`
        * Silence CC Duration: `15.0s`
        * Damage Taken Debuff: `+15.0%`
        * Damage Taken Debuff Duration: `15.0s`
        * Max Detection Range: `30.0m`
        * Max Detection Angle: `60`
        * Scan Delay: `1.0s`
        * Scan Color: `Magenta`
> Dev Note: The first sentry to be built as a CC tool than a lethal one. A turret that brings more utility for the team rather than pure damage.

### Syringe Tweaks:
* Heal Munitions Drain Syringe
    * Increased Heal Duration from `200s` to `300s`
        * Effectively increasing total heal from `120` to `180`
    * Increased Disinfection from `30%` to `40%`
> Dev Note: While this was a strong syringe, ammo was significantly more important than health in most cases. Hopefully this will incentivize players to weight their options.

### Class Fixes:
* All Class:
    * Switched description term of `Ranged Ammo` to `Gun Ammo`

* Marine:
    * Increased Gun Ammo Received from `+10%` to `+15%`
    * Increased Bleed Res. from `+90%` to `+100%`
        * Effectively making them immune to all bleed damage.
    * Decreased Projectile Armor from `+40%` to `+30%`

* Paramedic:
    * Increased Initial Ammo penalty from `-20%` to `-25%`

* Specialist:
    * Removed `Initial Gun Ammo` penalty
    * Added `Gun Ammo Received` penalty of `-20%`
    * Increased Ammo Capacity penalty from `-20%` to `-25%`
> Dev Note: Paramedic already a class with an initial ammo debuff. Specialist's weakness should be a bit more unique on its own. So they should no longer spawn in with little to no ammo. But instead receive less so their shots are more costly in the long run.

* Field Technician:
    * Increased Tool Ammo Received from `+25%` to `+30%`

* Abhuman:
    * Changed description to match with the other B-Company members.

### Enemy Tweaks:
* Scouts:
    * Increased Effective Range of EMP from `100.0m` to `200.0m`
    * Increased EMP Duration from `45.0s` to `47.5s`
> Dev Note: With the new tools and weapons to combat EMP blackouts, I believe the Scout needed a slight buff.

* Shadow Giants:
    * Increased Minimum Fog Radius from `3.0m` to `5.0m`
    * Increased Maximum Fog Radius from `6.0m` to `10.0m`
    * Increased Fog Density by `+25%`
> Dev Note: A Shadow Giant's infection fog should be larger size than the smaller variants.

* Children:
    * Decreased Explosion Damage from `6.0` to `5.0`
    * Increased Maximum Explosion Radius from `2.5m` to `3.0m`
    * Decreased Explosion Noise Minimum Range from `10.0m` to `7.5m`
    * Decreased Explosion Noise Maximum Range from `20.0m` to `15.0m`
    * Changed Explosion Sound Effect
> Dev Note: Less ear piercing loud and more consistent threat.

* Birthers:
    * Spawns Children upon death based on variant:
        * Birther: `6`
        * Birther Prime: `12`
        * Progenitor Mother: `18`
> Dev Note: Birthers should be a bit more dangerous once killed to prevent players from rushing them without consequences.

* Flyer:
    * Changed Explosion Sound Effect

### Miscellaneous Fixes:
* Fixed duplicate names in OfflineGear and FrontGearParts
* Changed README.md
    * Improved wording on all section
    * Fixed outdated information

---

### v2.3.4

### Emergency Hotfix:
* Fixed manifest.json:
    * Fixed an accidental typo that removed ExtraWeaponCustomization dependency

### Balance Tweaks:
* Foam Pistol:
    * Fixed the trait description showing the old trait of Armor Shred
    * Barricading requires only `2` shots instead of `3`
        * Just hit the door with melee after the second shot

* Wisp Launcher:
    * Fixed the gun's stat showing the incorrect precision multiplier
    * Decreased Max Ammo from `30` to `20`
    * Increased Friendly Fire Multiplier from `0.5x` to `0.8x`
> Dev Note: It seems like this gun is still performing a bit too well for how efficient the ammo economy is. Any more nerfs to this gun after this patch can potentially have the opposite effect.

### Mod Updates:
* Updated `ExtraWeaponCustomization` mod
* Updated `Informative Door Icons` mod

### Miscellaneous Fixes:
* Fixed README.md:
    * Not mentioning the new infection death penalty from previous patch

---

### v2.3.3

### Mod Updates + Additions:
* Added `Informative Door Icons` mod by HazardousMonkey
* Updated `ExtraWeaponCustomization` mod
* Updated `ExtraToolCustomization` mod
* Updated `EnemyAnimationFix` mod
* Updated `Spectate` mod
* Added `InfectionDeathPenalty` mod by Carb_Crusaders(me!)
    * Inflicts a `10%` infection penalty to players whenever they go down. This will add up(with other infections) until the `85%` limit
    * Can be treated with any disinfection method
    * Will be affected by `Infection Resistance` boosters, for example:
        * Courier class will receive double infection penalty
        * Paramedics class will be immune to the penalty
> Dev Note: Yes, I did create a mod specifically for this update. It's to combat a specific strategy where players would "heal" each other by dying then reviving through Paramedic. Additionally, this will bring another layer of challenge that incentivize players to stay alive, stick together more often, think twice before using AoEs, parry more often, and revive in safer situations. Disinfection packs/station, Medic Gun, and syringes are effective methods. This change is to also answer the recent increase in the player's power scaling with the new weapons, tools, and etc. I did not want to buff the enemies as that will rock the scales in a bad direction.

### Class Tweaks:
* Paramedic:
    * Class will "disinfect" `100%` themselves when loading into any rundown for the first time.
> Dev Note: Since this class is suppose to be immune to infection, it didn't make sense when certain rundowns forced infection at rundown startup.

* Prisoner:
    * Added other class's baseline stats
        * Infection Resistance: `+20%`
        * Hacking Proficiency: `-20%`
> Dev Note: This is in preparation of the InfectionDeathPenalty mod, as this class would earn 12.5% which is technically a stronger nerf than the others. To compensate for this buff, the hacking nerf that the other classes have is included too.

* Specialist:
    * Decreased Initial Ammo Penalty from `-40%` to `-30%`
> Dev Note: Previous nerf might have been too harsh. Basically had no ammo at the start to do anything at all.

### Weapon Tweaks:
* 4-B Nade Launcher AR:
    * Increased Direct Damage from `4.0` to `4.5`
    * Increased Effective Range from `21.0m` to `25.0m`
    * Decreased Hipfire Spread from `1.0x` to `0.6x`
    * Decreased Aim Spread from `0.4x` to `0.2x`
    * Decreased Shot Delay from `0.095s` to `0.07s`
> Dev Note: While the nerfs in the previous patch was warranted. It did make the gun's primary fire lose a lot of purpose. It basically became a glorified Burst Cannon lite, which is not my intention.

* Medic Gun:
    * Increased Mode 2's DoT Stagger Multiplier from `30.0x` to `40.0x`
    * Increased Mode 3's Armor Shred from `-20%` to `-30%`

### Booster Tweaks:
* Infection Resistance `Muted` Booster:
    * Increased Resistance bonus from `+10%` to `+15%`
* Infection Resistance `Bold` Booster:
    * Increased Resistance bonus from `+15%` to `+20%`
* Infection Resistance `Aggressive` Booster:
    * Increased Resistance bonus from `+20%` to `+25%`
> Dev Note: In response to the new death penalty; from 45% to 60% plus the 20% baseline bonus that all classes have. This should be a viable option where infection is a common mechanic.

### Miscellaneous Fixes:
* Fixed README.md on classes to reflect the class tweaks from v2.3.1
    * Added Booster and Syringe section
    * Switched the mega thread links from `Issue` to `Discussion` tab

* Removed v2.0.0 from the CHANGELOG.md(done to make more space)
    * You can check on github repo for old notes

---

### v2.3.2

### Mod Updates + Additions:
* Updated `BetterBots` mod

### Balance Tweaks:
* Beam Rifle:
    * Decreased Glow Intensity from `0.05` to `0.01`
    * Decreased Glow Range from `10.0m` to `8.0m`
> Dev Note: Eye strain nerf.

* Search and Rescue Tool: **Improvement**
    * Increased Charge Timer from `1.0s` to `2.0s`
    * Item Projectile Speed/Distance is based on `Charge Amount`:
        * Charge(<20%): `5.0m`
        * Charge(20%-50%): `10.0m`
        * Charge(50%-90%): `20.0m`
        * Charge(>90%): `40.0m`
    * Fixed visual bug with ammo counter when swapping
    * I'm aware of another visual bug with ammo counter at 0%. Does not affect gameplay.
> Dev Note: It's still a bit too awkward to use this tool as players have found it difficult to control the speed/distance these items fly. This QoL change should significantly improve usage.

* Exterminatus Flamer:
    * Increased Bullet Cost per shot from `1.0` to `2.0`
    * Decreased Clip Regen from `5.0` to `4.0` per second
    * Increased Clip Regen Delay from `5.0s` to `7.5s`
    * Decreased Glow Intensity from `0.05` to `0.01`
    * Decreased Glow Range from `10.0m` to `8.0m`
> Dev Note: This change is to reign in the flamer as it's very effective against hordes, which is good! But it might be a bit too good as it had low consequences when utilized. Other than eye strain...

* RYN0 Annihilator:
    * Decreased Inner Radius from `7.5m` to `7.0m`
    * Decreased Outer Radius from `15.0m` to `14.0m`
    * Increased Maximum Explosion Damage from `700.0` to `800.0`
    * Explosions completely ignores Armor for all targets, including friends!
> Dev Note: Because why not? At this point only the Demolitionist and/or Shock Trooper with 3 Explosion Res. boosters can survive. Maybe the Abhuman... big maybe.

### Miscellaneous Fixes:
* Fixed typos and mistakes within v2.3.1's changelog

---

### v2.3.1

### Mod Updates + Additions:
* Updated `EnemyAnimationFix` mod
* Updated `SpreadStartingAmmo` mod
* Added `NoBrokenBotGear` mod by JarheadHME
    * It has come to my attention with bots being broken in the lobby that prevents dropping down a rundown. Caused by bots having weapons/tools that have been changed and it is loading something that doesn't exist. What you can do:
        * Delete the `BotGear.json` file within `BepInEx/GameData/Favorites/Botgear.json` of your profile.
        * Or search the file in `Edit Config` and delete the file.
        * Or try to change the gear before the bot disappears within the lobby(unreliable).

### Class Tweaks:
* Updated `GTFuckingXP` mod
* Switched all class `Ammo Cost Efficiency` bonus/penalty with `Ammo Capacity` bonus/penalty
* Switched all class `Tool Cost Efficiency` bonus/penalty with `Tool Capacity` bonus/penalty
> Dev Note: All classes will receive a more universal ammo/tool efficiency. Those that had the original positive values will be nerfed while vice versa for negative values. This should help balance out issues where classes who had high/low efficiency aren't punished/rewarded for resupplying.

* Marine:
    * Replaced `+20% Initial Ranged Ammo` bonus with `+10% Gun Ammo Received`

* Field Technician:
    * Replaced `+50% Initial Tool Ammo` bonus with `+25% Tool Ammo Received`
> Dev Note: While the loss of initial ammo is something to adjust to, the increased ammo gain will give them better potential long-term. These bonuses will stack well with Quartermaster's/Booster's Resupply efficiency

### Balance Tweaks:
* Updated `ExtraWeaponCustomization` mod
* Beam Rifle:
    * Increased Damage Accumulation from `0.5%` to `2%` per hit
        * Shots require `50%` less to reach full damage potential for body and weakspot hits
    * Increased Damage Accumulation Cap for Body Shots from `1.5x` to `2.0x`
    * Increased Damage Accumulation Cap for Weakspot Shots from `2.0x` to `3.0x`
    * Increased Max Ammo from `1000` to `2000`
    * Increased Base Ammo Received from `200.0` to `400.0`
> Dev Note: After some more testing, I found the overall damage to be a little low for how expensive the gun's bullet economy is. Instead of simply buffing the base damage, I opted to reward players for choosing to stay on one target during a burst.

* Semi/Full-Auto AK Rifle
    * Changed name from `Semi/Full-Auto Rifle` to `AK Platform Rifle`
    * Decreased Direct Damage from `7.5` to `7.0`
> Dev Note: A tad bit overperforming with the new changes from previous patch

* 3-B Carbine: **Rework**
    * Increased Direct Damage from `3.4` to `4.0`
    * Decreased Max Ammo from `453` to `400`
    * Switch between `2` modes(Semi-Auto & 3-Burst Fire):
        * 3-Burst Fire:
            * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
        * Semi-Auto:
            * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])    
* 4-B Nade Launcher AR:
    * Decreased Direct Damage from `5.0` to `4.0`
    * Increased Grenade Ammo Cost from `15` to `20`
    * Decreased Maximum Explosion Damage from `45.0` to `40.0`
    * Decreased Minimum Explosion Damage from `25.0` to `20.0`
    * Decreased Max Ammo from `400` to `300`
    * Increased Reload Time from `2.2s` to `2.4s`
    * Switched Nade Launcher from `Reserve Ammo` to `Clip Ammo`
        * It will pull from reserve to make up for the grenade ammo cost
> Dev Note: This gun is too overtuned and does almost everything in one. While I am never a fan of straight up nerfs. Unfortunately, it is warranted.
* 5-B Bullpup: **Rework**
    * Decreased Direct Damage from `3.1` to `3.0`
    * Decreased Max Ammo from `508` to `500`
    * Switch between `2` modes(Full-Auto & 5-Burst Fire):
        * 5-Burst Fire:
            * Activated by using specific keybind trigger(Default Keybind: KeypadPlus[KeyConfig2])
        * Full-Auto:
            * Activated by using specific keybind trigger(Default Keybind: KeypadEnter[KeyConfig1])
> Dev Note: This is a bit of a balancing act for these three burst weapons. They should be more consistent with each other. Also the Marine class is getting a buff to ammo receive efficiency. Hopefully it should balance the numbers a bit.

* Wisp Launcher:
    * Decreased Max Ammo from `40` to `30`
    * Decreased Wisp Death Shrapnel Count from `10` to `6`
    * Decreased Precision Multiplier from `1.1x` to `1.0x`
    * Increased Clip Regen Delay from `16.5s` to `25.5s`
    * Switched Regular Quill Targeting Mode from `Weakspot` to `Body`
    * Switched Death Quill Targeting Mode from `Weakspot` to `Normal` (aims for the head if it exists, then the body. Does not aim for tumors)
    * Switched Targeting Priority from `Angle` to `Distance` except for death quills(to prevent homing failures)
> Dev Note: It's a little too good at its job. So I will have to reel in its power, hopefully without completely removing its usefulness.

* Choke Mod Shotgun:
    * Increased Direct Damage from `7.0` to `9.5`
    * Increased Clip Size from `5` to `6`
    * Increased Effective Range from `20.0m` to `30.0m`
    * Increased Precision Multiplier from `0.9x` to `1.05x`
> Dev Note: This gun was originally very powerful, so I had to adjust it. But the significant changes may have hurt this gun too much. 

* Missile Sentry:
    * Added `Max Ammo(15)` into the trait description.
        * There is currently a bug where the max ammo is shown as `5` when it is actually `15`

* Nano Gauss Rifle:
    * Increased Projectile Hit Size Bonus from `+0.2m` to `+0.5m`

* W-Pen Sniper Rifle:
    * Added `ThickBullet` Property:
        * Increased Bullet Hitbox by `+0.15m`

### Miscellaneous Fixes:
* Fixed numerous typos and errors within v2.3.0's CHANGELOG.md
> Dev Note: There was a number of wrong information written in the previous update. A mistake on my part for not double checking...
* Removed old changelog for character space limit.
    * Please check old changelog at [Github](https://github.com/Heaveness/GTFriendlyO/blob/main/GTFO%20OLD%20CHANGELOGv220.md)

---

### v2.3.0

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
    * Direct Damage: `1.5`
    * Reserve Ammo, no reload
    * Clip Regen up to `100` after Shot Delay
    * Max Ammo: `2000`
    * Clip Size: `100`
    * Pierce Limit: `1` 
    * Fires `1` continuous beam costs `100` rounds
    * Damage increases continuous hitting a single target for the whole beam. 
        * Up to `2.0x` damage cap for normal shots as it stacks 1 at a time
        * Up to `3.0x` damage cap for weakspot shots as it stacks 2 at a time
        * Duration lasts `2.5s` then rapidly decays. Continued hits from the user will refresh the duration
    * Shot Delay: `2.0s`
    * DoT Damage: `1.0`
    * DoT Duration: `10.0s`
    * DoT Tick Rate: `2`
    * DoT Stack Limit: `100`
    * Shrapnel Count: `1`
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
    * Changed name from `Semi-Auto Rifle` to `Semi/Full-Auto AK Rifle`
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
    * Switched `ArmorShred` to `ShotModDebuff` property:
        * Applies `+30%` increased base damage(excluding precision & stagger) debuff on an enemy target for all sources
> Dev Note: With a lot of new options to foam targets, the Foam Pistol lost a lot of its place in the roster. So I am switching the armorshred to a "Increase Damage Taken" debuff on the target that is currently unique to this gun only.
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
> Dev Note: I want to slightly lower the Burst turret's clunkiness to be a bit more reliable on maps that have tight corners.
* Missile Sentry:
    * Added text description for traits
    * Fixed explosion not having friendly fire multiplier. *Oopsie...*
    * Increased Friendly Fire Multiplier from `-50%` to `-70%`
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