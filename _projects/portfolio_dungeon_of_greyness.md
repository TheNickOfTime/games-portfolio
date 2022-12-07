---
title: Dungeon of Greyness
image: '/assets/portfolio_dungeon_of_greyness/CombatDesign_Thumbnail.png'
---

# Introduction
“Dungeon of Greyness” is a game prototype, with a focus on combat design, that I built from the grround up over the course of a semester. My goal for this project was to focus on the various nuances of what makes combat feel engaging and fun, and flesh these elements out, week-by-week.

Using the Unity Engine, I designed and scripted (C#) everything in this project. This extends from the levels, the core gameplay, player combat & enemy functionality, to all the underlying systems that make the game work. Virtually all art and music was borrowed/copied in order to focus on the mechanical aspects of the game.

<br>

![Gallery](/assets/portfolio_dungeon_of_greyness/Screenshots/CombatDesign_Screenshot_01.png)

<br>

# Summary

## Challenge
Since this project was going to be a semester-long work, choosing what to do was particularly difficult. The only real guidelines for my project were that it had to be 2D and the combat had to be based on an existing, good quality game. Keeping scope in check would be difficult, as it is easy to plan to do too much when given a large amount of time.

An additional challenge of this project being semester-long was writing and maintaining a clean and clear codebase. This was not a requirement set by the class, but more of a personal necessity to maintain sanity over the long-term.

## Solution
My initial concept was a game inspired by the combat of Hyper Light Drifter. Unfortunately, I wasn’t able to find a proper character sprite set, so I decided I would hand draw each frame from Hyper Light Drifter. This was dumb and took up so much time, however, I did leave this project with a newfound appreciation for the craft of pixel art.

To keep the scope manageable, I landed on the concept of having individual, smaller rooms with between 1 to 3 waves of enemies each. Progressing through the rooms would gradually introduce the player to different and harder enemies. This would allow me to create as many or as few levels as I wanted/could, without having to cut content.

I made a limited, but diverse set of enemies. There are two grunt-level melee enemies, one harder “Lieutenant” level melee enemy, and a tricky ranged enemy. In addition to these standard enemies, there is a final boss that possesses all the traits of these enemies plus more.

-----

## Result
My combat project ended up as Dungeon of Greyness. It is a fairly complete, but small prototype that holds a reasonable amount of content (~15 – 20 minutes for new players) and progression. You play as a traveler who fights through seven high-tension rooms filled with aggressive enemies. You are aided by a stranger with upgrades, but little else.

Overall this project was a fantastic experience, both personally and educationally. I was finally able to spend more than a few weeks on a project and focus on refining gameplay in a meaningful way. I learned a ton as I went along and thankfully I wrote some of the cleanest code I have so far which made evolving the game a breeze. The feedback I have received from playtesters has been pretty positive and I am glad people have found it to be an enjoyable experience!

<br>

# Highlights

![Player](/assets/portfolio_dungeon_of_greyness/GIFs/CombatDesign_PlayerMovement.gif)
## Player
The inspiration for the player combat of this game was Hyper Light Drifter. This is pretty obvious looking at the character because I straight up hand copied each frame of each animation from some gameplay footage I took of HLD. I wanted to stay away from this initially, but unfortunately, I found it impossible to find a top-down game sprite-set that had the dynamic and powerful feeling that the animations of HLD have.

At a base level, the player has a basic attack that can be chained up to three times, increasing in damage each hit of the combo. Near the start of the game, the player is given the ability to dash. The dash allows the player to be fluid in combat, as well as escape sticky situations since there is an invulnerability window during the dash. Later, the player unlocks two additional upgrades - Super Slash and Super Dash. Super Slash allows the player to hold the attack button to charge an attack that does an impressive amount of damage that ignores shields. Super Dash similarly allows the player to hold the dash button to charge up a dash that both slightly damages as well as momentarily stuns enemies.

The goal was to make the player feel powerful from the start, but give them more ways to deal damage as the game progressed. It is pretty easy to die, but death is not meant to be punishing in this game. You automatically respawn within a second or two of dying at the start of the room you died in. This allows the player to learn from mistakes and avoid frustrations that come with difficulty.

<br>

## Enemies

![Slime](/assets/portfolio_dungeon_of_greyness/GIFs/CombatDesign_Slime.gif)
### Slime
The Slime is the most basic enemy of the bunch. It moves quickly, deals a very small amount of melee damage, and on its own, is barely a threat. 2 standard hits can eliminate this weak enemy. In a group, they can quickly overcome the player though.

![Skeleton](/assets/portfolio_dungeon_of_greyness/GIFs/CombatDesign_Skeleton.gif)
### Skeleton
The Skeleton is functionally the same as the slime, however, it deals more damage and has more health. These traits make it a bigger threat to the player than the slime, but they become a pretty minor threat after the first few. This is intentional.

![Knight](/assets/portfolio_dungeon_of_greyness/GIFs/CombatDesign_Knight.gif)
### Knight
The Knight, unlike the Slime or Skeleton, is a bit more intelligent. Since the knight has a shield, it will block all attacks from the front. The player has to methodically approach this enemy, either waiting for or creating an opening to dash behind it and get a few hits in. This enemy hits very hard, so it is important for the player to keep on their toes. Fortunately, it moves pretty slow and the attacks have pretty clear indicators they are coming.

![Wizard](/assets/portfolio_dungeon_of_greyness/GIFs/CombatDesign_Wizard.gif)
### Wizard
The wizard is the most unique enemy and perhaps the hardest. It has a ranged attack set, but rather than firing projectiles, the Wizard spawn hazardous tile patterns around the player. The player has a relatively small window to decide if they should stay put, move a bit, or dash far away. Rather than walk around, this enemy teleports from position to position, this can make it difficult to eliminate this enemy quickly. This enemy exists to disrupt the more predictable melee enemies.

![Boss Knight](/assets/portfolio_dungeon_of_greyness/GIFs/CombatDesign_BossKnight.gif)
### Boss Knight
The Boss Knight is in appearance a palette swap of the regular Knight, however, it has a few different tricks up its sleeve. Unsurprisingly it has the largest health pool of all enemies and does the heaviest damage. It possesses melee attacks inherited from the Slime, Skeleton, and Knight, as well as the Knights shield blocking trait. It can also execute ranged attacks inherited from the Wizard and teleport away if it gets hit too many times in a row. This boss enemy also has the unique ability to spawn grunt level enemies around it to distract the player.

All of these traits make this enemy very dangerous. These different traits are introduced in 3 different states based on the boss’s health. Most players will fail at least the first time, but since death is not meant to be punishing, the player can learn the patterns fairly quickly and defeating it is a very rewarding event.

<br>

## World
While combat was the focus of this project, I found that the world and level design were deeply integrated into this system. For example, the player cannot swim, so water is a threat – almost another enemy depending on the situation. Additionally, the size and layout of a room can create obstacles that the enemies do not on their own. Because of this, I took time making each room to be unique in its design and what types of enemies spawn when and where.

Aside from how the world relates to the combat, I wanted the pacing and progression of the world to feel right. Since the general flow of my game was moving room to room, I noticed it felt very tedious to move directly from one combat scenario to another. A solution for this was putting in “transition levels” that lack any combat. These transition levels were also a fun way to add some personality to the game as well as provide the player with some simple side-objectives that do a good job of breaking up gameplay.
