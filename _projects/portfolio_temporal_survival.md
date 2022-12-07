---
title: Temporal Survival
image: '/assets/portfolio_temporal_survival/TemporalSurvival_Thumbnail.jpg'
---

## Introduction
Temporal Survival was the product of a game jam that was put on within the QA department at Naughty Dog in 2021. My team consisted of myself as the game designer, Sami Hagerman as the artist, Phillip Menses as the audio designer, and Aiden Thurston as our producer & design support person.

The prompt for this project was “Time” – something must have been in the water since nearly everyone on the team gravitated towards a sci-fi theme with mechanics centered around concepts of relativity, aging rapidly, and using technology to combat this.

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed//xZrxQmIr9OM' frameborder='0' allowfullscreen></iframe></div>

<br>

-----

<br>

## Overview
As the game starts the player is presented with a brief log – it explains that the player has crash landed on a planet where time moves differently, due to temporal energy that is emitted by crystals covering the surface. The player is presented with a difficult decision to balance – the crystals recharge the player’s suit and protect them from rapidly aging, but the player must also research the crystals to more permanently survive on the planet.

### Mechanics
The gameplay loop looks like this:

1. The player exits their shelter, entering the harsh temporal environment of the planet. Your time is limited out here before your suit charge is drained, and you begin aging rapidly – eventually dying.
2. The player has to mine crystals from the surface of the planet. The mining process is a minigame:
    - The player presses the triggers on the controller, using either haptics, audio, or visual aids to find the “sweet spot” on each trigger (randomized every time).
    - The player has to maintain the triggers in this “sweet spot” for a length of time to successfully mine the crystal.
3. Once the player has a crystal in tow, they can choose to mine more (weighing how much time you have left on your suit charge) or head back to the shelter.
4. Once back in the shelter, the player can use their crystals to either recharge their suit, or to progress research on the temporal anomaly. It’s a balancing act.
5. Once the player successfully completes research, the player reaches the win condition. If the player fails to manage what they use their crystals for and ages too much, the player dies at the ripe age of 80-something and it is game over!

### Mining Minigame
The minigame is my favorite aspect of this jam. When this project was made, the concepts and use cases for the Dual Sense 5’s adaptive triggers were fresh on my mind. Unfortunately the Unreal Engine does not support Playstation Controllers out of the box so I made do with an Xbox controller and modulating the frequency of the haptic feedback.