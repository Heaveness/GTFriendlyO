# GTFriendlyO

## Description

A major overhaul of GTFO's vanilla gameplay, designed for a more casual but still fun and challenging experience with friends.

As a long-time GTFO player, I've felt the base game lacked a bit of variety in certain aspects of its gameplay. After running several Rundowns with friends, we all agreed the game needed a bit more spice. This mod focuses on creating a more casual-friendly co-op experience without removing all of the tension or challenge from the game. This is NOT a hardcore or hyper-realism mod setup, nor will it ever be. Instead, it makes GTFO more accessible by giving players additional "tools" to tackle the depths. The enemies have also received some love too, so it's not completely one-sided.

Heavy inspiration: FriendlyGTFO by EcoLight and Duo Trials by ProjectZaero
> Please note that I took the syringe customization settings from Duo Trials to reverse engineer on how it was made. I have made some changes, but the overall credit belongs to the ProjectZaero. Currently working on a re-work of the syringes.

This project has been in the works for years. Until now, it's only been shared privately with my friends. Now, I'm releasing it publicly for others to enjoy as well. Play together or die together!

## Important

* Please note that this is only a baseline modpack, more mods will be considered in the future. Mainly mods needed for a better experience. **Stay tuned!**

* Can be played Vanilla with other mods with this mod-pack, especially client-side mods.

* Most likely will NOT be compatible with other custom Rundowns or modpacks that changes the same Datablocks. Otherwise, give it a try and let me know.

## Major Changes

###### Players:

* Increased base Health: `25.0 -> 60.0`
* Increased base Regen Cap: `20% -> 30%`
* Increased Regen Delay after Damage: `5.0s -> 10.0s`
* Increased Regen Delay: `1.0s -> 5.0s` 
* Increased Regen per Second: `0.2 -> 1.0`
* Increased Friendly Fire Damage: `50% -> 80%`
* Increased Fall Damage Min/Max Height: `4.0m/20.0m -> 6.0m/30.0m`
* Increased Fall Min/Max Damage: `2.0/15.0 -> 10.0/40.0`
* Increased base Walk/Sprint/Crouch/Ladder Spd. and Footstep Length by `0.5-1.0`. 
* Rewored Stamina Cost across the board. Overall higher cost in combat, but faster regen out of combat.
* Higher starting ammo and cap.
* Decreased ammo supply efficiency from Ammo-Packs.

###### Classes:

* All classes have distinct roles with pros and cons. There is no leveling system, all classes get their stats at the start.
* Meant to be played with 2+ players.
* All classes can do damage, some do it better than others. Boosters/Syringes can be used to further buff or debuff attributes.
* `Damage` roles are classes that specialize is mainly doing damage, but they tend to be more fragile.
* `Tank` roles are classes that specialize on taking damage while also dishing out some of their own, but they tend to be on the slow side.
* `Support` roles are classes that specialize on helping the team, but they lack either offensive or defensive capabilities.
> Dev Note: B-Company Division is meant for joke classes, never will be balanced or realistic. So have fun with them.

| CLASS       		| ROLE      | DIVISION  | STRENGTHS 	 											          | WEAKNESSES																      |
|-------------------|-----------|-----------|:-------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| Marine 			| Damage 	| Combat 	| Accurate; mid-to-long range; consistent damage                      | Low melee armor & damage                                                      |
| Spec Ops 			| Damage 	| Combat 	| Stealth melee; high damage; high movement speed                     | Low base HP; very fragile                                                     |
| EOD Specialist	| Damage 	| Combat 	| Crowd control AoE; big explosions; explosive resistance             | Poor tech skills (terminal, hacking, sentries)                                |
| Shock Trooper 	| Tank 		| Combat 	| High armor; strong base HP; fast regen speed                        | Low damage overall; relies on shotguns & melee; slow movement speed           |
| Paramedic 		| Support 	| Support 	| Infection immune; high revive speed & health; fast regen delay      | No offensive benefits; low starting & max ammo                                |
| Quartermaster 	| Tank 		| Support 	| High ammo efficiency; strong starting ammo; high HP regen cap       | Very slow movement speed; low damage (except with MGs)                        |
| Tool Specialist 	| Support 	| Support 	| Effective & efficient with all tools and items                      | Low starting & max ammo; no offensive benefits                                |
| Field Technician 	| Damage 	| Support 	| Stronger & faster sentries; fast terminal & hacking skills          | Low base damage (melee & ranged); low starting ammo                           |
| Prisoner 			| Neutral 	| B-Company | No major strengths; closer to vanilla experience                    | No major weaknesses; closer to vanilla experience                             |
| HEL Diver 		| Damage 	| B-Company | Strong HEL gun damage; fast terminal & hacking; high movement speed | High friendly fire damage; fragile; low base HP & regen cap                   |
| Abhuman 			| Tank 		| B-Company | Very high base HP; strong melee damage; extended hitbox/range       | Poor with terminals & sentries; low starting ammo; reduced movement           |
| Deprived 			| Damage 	| B-Company | High resistances; strong damage; projectile armor; fast objectives  | Extremely fragile esp. against melee; low starting ammo                       |

###### Weapons:

- All of the Main and Special weapons have either been overhauled, reworked or tweaked.
- Muzzle flash has been mostly removed as my friends and I am photosensitive.
- Significantly changes were made to create synergies between weapons and classes.
- Promotes more build diversity and team compositions.
- Silence CC does not mean silent weapon, it's the capability to temporarily disable some enemy abilties such as non-boss tongues.
- DoT stands for Damage-over-Time effect that deals damage based on ticks per second.
- Reserve Ammo means there is not reloading, as the weapon utilize the whole ammo reserve.

| ORIGINAL NAME			| NEW NAME							| TRAIT															| BALLISTICS		|
|-----------------------|-----------------------------------|:-------------------------------------------------------------:|:-----------------:|
| Shelling S49        	| Shelling Tracker Pistol			| Tags target on hit											| Hitscan			|
| Shelling Nano       	| Shelling Foam Pistol				| Foams targets; shreds armor					        		| Hitscan			|
| Bataldo 3RB	 	  	| Bataldo Revolver					| Hold trigger for rapid fire; richochet on terrain             | Hitscan			|
| Raptus Treffen 2    	| Raptus MP2						| Full-auto; 50-round mag				            			| Hitscan			|
| Raptus Steigro      	| Raptus Reserve MP1				| Reserve ammo; no reload               						| Hitscan			|
| Accrat Golok DA     	| Accrat 5-B Bullpup				| 5-round burst fire            								| Hitscan			|
| Van Auken LTC5      	| Techman Hemostasis Medic Gun		| Heal allies / Venom enemies; silence CC       		        | Projectile		|
| Accrat STB          	| Omneco Tracker PDW				| Tags target; thermal scope       								| Hitscan			|
| Accrat ND6          	| Van Auken Heavy SMG				| Standard bullets												| Hitscan			|
| Van Auken Cab F4    	| Accrat 3-B Carbine				| 3-round burst; Standard bullets	                            | Hitscan			|
| TR22 Hanaway        	| Hanaway DMR						| Standard bullets												| Hitscan			|
| Hanaway PSB         	| Hanaway Double-Tap				| Standard bullets												| Hitscan			|
| Malatack LX         	| Van Auken Heavy Rifle				| Standard bullets												| Hitscan			|
| Malatack CH 4       	| Mastaba Explosive Shrapnel Rifle	| Explosive burst; charge-up; shrapnel              			| Projectile		|
| Drekker Pres Mod 556	| Malatack Assault Rifle			| Standard bullets												| Hitscan			|
| Buckland SBS III    	| Buckland Triple-Barrel			| Standard bullets												| Hitscan			|
| Bataldo J 300       	| Buckland Hemorrhage Shotgun		| Standard bullets; applies DoT bleed                           | Hitscan			|	
| Bataldo Custom K330 	| Bataldo Single Slug				| High-precision slug; fast reload                              | Hitscan			|
| Malatack HXC        	| Malatack AR-30					| Standard bullets 												| Hitscan			|
| Drekker CLR         	| Techman Exp. Smart Rifle			| Lock-on required; auto-aim homing		                    	| Projectile/Homing	|
| Buckland S870       	| Bataldo Pump Action				| Standard bullets												| Hitscan			|
| Buckland AF6        	| Buckland Reserve Hemorrhage Shotty| Reserve ammo; no reload                                       | Hitscan			|
| Buckland INEX Drei  	| Mastaba Explosive Shotgun			| Explosive rounds; charge-up                                   | Projectile		|
| Buckland XDIST2     	| Buckland Choke Shotgun			| Standard bullets												| Hitscan			|
| Mastaba R66         	| Bataldo Heavy Revolver			| Hold trigger for rapid fire; richochet on terrain             | Hitscan			|
| Techman Arbalist V  	| Raptus LMG						| Standard bullets                                              | Hitscan			|
| Techman Veruta XII  	| Raptus Reserve HMG				| Reserve ammo; no reload                                       | Hitscan			|
| Techman Klust 6     	| Mastaba Explosive Shrapnel Cannon	| Explosive burst; charge-up; shrapnel					    	| Projectile/Gravity|
| Omneco Exp1         	| Hanaway Hemorrhage HEL			| Standard bullets; applies DoT                                 | Hitscan			|
| Shelling Arid 5	  	| Shelling Bolt Pistol				| Standard bullets                                  			| Hitscan			|
| Drekker Del P1      	| Omneco Tracker Rifle				| Tags target on hit                                            | Hitscan			|
| Köning PR 11        	| Van Auken W-Pen Sniper Rifle		| Wall-penetration bullets                                      | Hitscan			|
| Omneco LRG          	| Techman Nano-Payload Gauss Rifle	| Nano-Burst shrapnel on kill seeks target                      | Hitscan/Projectile|

#### Melee:

* All four melee types have been reworked to be more distinct from each other.
* Sledgehammers and Bats are meant for players who prefer loud encounters.
* Knives and Spears are meant for players who prefer quiet engagements.
* There is another mod called Parry, which is not included in this mod setup. But it will be for the mod-pack.
> Dev Note: Parry can be used on melee or projectile damage, latter can send the projectile back to sender. 

| TYPE       	| ROLE      | TRAITS  			| STRENGTHS 	 								| WEAKNESSES								    	|
|---------------|-----------|-------------------|:---------------------------------------------:|:-------------------------------------------------:|
| Sledgehammer	| Loud 		| Armor Piercing	| High Heavy Damage & Stagger Multplier		    | High Stamina Cost, & Sluggish						|
| Knives 		| Silent 	| Bleed Effect		| High Stealth/Backstab Damage & Fast Spd.		| Low Base Damage & Short Range						|
| Spears		| Silent 	| Tagging Effect 	| High Hitbox Range & Precision Multiplier		| High Stamina Cost, & Long Charge Time				|
| Bats 			| Loud 		| Explosive Kills 	| High Light Damage & Low Stamina Cost			| Low Precision/Stealth Damage, & Low Heavy Damage	|

#### Tools:

* Most tool gear & items have received some tweaks. Overall increase in carrying capacity for items and sentry ammo.
* This section will mainly showcase sentries.
> Dev Note: The ResourceStacking mod will be an important upgrade for consumables.

| SENTRIES      | RANGE 	| QUIRKS		  									| STRENGTHS 	 									| WEAKNESSES										|
|---------------|-----------|---------------------------------------------------|:-------------------------------------------------:|:-------------------------------------------------:|
| Burst Turret	| Medium	| Burst Fire, Shot Delays cause leaks in defense	| Consistent Damage, & Reliable						| Easily Overwhelmed & Requires Sufficient Space	|
| Auto Turret 	| Short	 	| Holds Choke Points, but wastes a lot of bullets	| High Stagger Damage, & High Ammo Cap				| Poor Accuracy, & Very Ammo Hungry					|
| Sniper Turret	| Long		| Alt. to snipers, but fires at Tagged targets ONLY	| Very High Single-target Damage, & Ammo Efficient	| Poor Defense, & Long Setup						|
| Shotgun 		| Short		| Destroys Choke Points, but struggles w/open rooms	| High Close-Range Damage, & CTRL+ALT Delete chokes	| Placement Dependent, & Quite Ammo Hungry			|

#### Enemies:

* All enemies have had their base and limb health increased to keep them balanced against the players' new power scaling.
* Minimum base health increase of 20.0 while larger elites and bosses received massive health increase.
* Each Enemy/Variant received new quirks to improve their strengths and solidify their identities.
* Some names were changed to keep a consistent identification. For example: `Shooter -> Needler`

| ENEMIES      				| ABILITIES/TRAITS  													| NOTES																						|
|---------------------------|:---------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| Strikers					| Higher HP, but less damage											| N/A, just punch'em.																		|
| Needlers(Shooter) 		| Stronger overall damage, but more fragile								| N/A, just shoot'em.																		|
| Large Strikers  			| Tongue grabs player to its melee range; cannot parry the pull			| Loves pulling teammates out of bioscans, either kill or disable(Medic Gun or Foam Pistol).|
| Scouts 					| EMP(45.0s) after scream, invul. during EMP wind-up					| EMPs disable all, but glowsticks, fog repellers, and tripmines. Try Tool Specialists!		|
| Birther 			        | Increased HP; Birth Children that will explode on death				| Kill the babies first, then kill the mothers fast.										|
| Stalkers(Snatcher) 		| Significant HP increase, snatched players will take damage        	| Takes longer to kill and can kill players now. They should not be ignored.				|
| Bloom Needlers & Flyers	| Inflicts bleed(50% Chance) for 2.5% damage over 5.0s; stackable		| Bloom Needlers are high-priority targets otherwise team member will suffer major damage.	|
| Tanks						| Significant increase in HP & high knockback; door buster				| Significantly longer to kill, their knockback is annoying, and don`t close doors on them.	|

* Variants will have traits and abilities listed above while also having extra perks mentioned below.

| VARIANTS      | TRAITS 																	|
|---------------|:-------------------------------------------------------------------------:|
| Large 		| Signicantly increased health and stagger resistance						|
| Charger 		| HP Regen(80% Cap) if not damaged within 5 seconds, damage resets timer	|
| Nightmare  	| Inflicts infection on all attacks	& scout screams							|
| Shadow 		| Mainly unchanged, slightly increased Tag time by 3s						|
| Child			| Explode on Death, can cause a chain reaction								|

## Extras:

* If you have any feedback, please let me know through the Github Link: [Here](https://github.com/Heaveness/GTFriendlyO).
    * Open a ticket under "Issue" tab if you are unsure where to send feedback. 
* Check out the Thunderstore page: [Here](https://thunderstore.io/c/gtfo/p/Carb_Crusaders/GTFriendlyO/).
* Check out the wiki pages for more information on each major feature: [Here](https://thunderstore.io/c/gtfo/p/Carb_Crusaders/GTFriendlyO/wiki/).
* If you really liked the mod-pack, give it a thumbs up on Thunderstore. Try it out with friends or randoms!