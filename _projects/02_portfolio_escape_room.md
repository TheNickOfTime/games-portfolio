---
title: Escape Room
permalink: /portfolio/escape-room
image: '/assets/portfolio_gravity_box/GravityBox_Thumbnail.png'
---

<div style="text-align:center">
    <a href="https://github.com/TheNickOfTime/design-challenge-jan/releases/download/v1.0/design-challenge-jan.zip" target="_blank" class="button button--primary">Download</a>
    <a href="https://github.com/TheNickOfTime/design-challenge-jan" target="_blank" class="button button--primary">Source</a>
</div>

<br>

<p><iframe src="https://www.youtube.com/embed/69xydia0joM" loading="lazy" frameborder="0" allowfullscreen></iframe></p>

# Summary
This project was made using the [Godot Engine](https://godotengine.org/) during a monthly design challenge, with the following prompts:
- Thematic Prompt: Machines
- Mechanical Prompt: Multi-step Puzzle

I started with some pretty specific inspirations with this project. The most obvious is Portal 2 - it's a masterpiece of a game and the co-op levels are a blast. I was also inspired by It Takes Two, primarily by how each character in that game tends to have a specific role and/or abilities. So essentially I wanted to make a puzzle game where you control two unique characters, and using their abilities you have to solve various micro-level puzzles to solve a macro-level room puzzle.

# Characters

## Shift
One of the characters is a "Shape Shifter." It has three states:
1. Normal - The default state
2. Squashed - The character becomes shorter, but also wider.
3. Stretched - The character becomes taller, but also skinnier

Additionally this character has the ability to pick up certain interactable objects - like a weighted cube.

## Divide
The other character has the ability to split in two. Uniquely the characters mass is relatively maintained when dividing, and the subsequent twins are much shorter. The player directly controls the primary twin, and commands the secondary twin via a ping/waypoint system.

Additionally when splitting, the primary twin is located on top of the secondary twin. Since neither character can jump this presents the player with a rare opportunity to travel vertically.

## Together
With these unique characteristics of both characters, each one ends up playing specific roles within the environment. The players can even literally piggy-back on each other's mechanics. For example, the Shift Character can become squashed, and the Divide Character can climb on top to be carried to greater heights!

# Puzzle Mechanics
I wanted making levels to be pretty straight forward, almost drag and drop w/ no special scripting required. What I came up with is a system of cause and effect, which I named "triggers" and "triggerables." What this allows is you to place any one "cause" in a level, and it having any effect(s).

## Triggers
In this prototype there are two types of triggers - Buttons & Lasers. Each trigger has a power-line you can attach to it so it is clear what it will effect in the world.

### Buttons
These are pretty straight-forward - you step on it (or place another object with mass) and it does things!

### Lasers
Lasers operate physically in the world - if something is in the way, the laser won't be able to reach it's destination.


## Triggerables
These are what are on the other end of triggers. Well, they can be - you can also have them operate independently if needed! These are what do things.

### Platforms
Since neither player can jump, introducing verticality via moving platforms was necessary. Additionally these can be set up to move horizontally as well.

### Doors
What more is there to say, its a door!

### Lasers
The on/off state of a laser is a triggerable!

### Conveyors
These didn't make it into the final product unfortunately (ran out of time to design levels). But these move players & other objects in one direction. I'm excited about the future potential of these.