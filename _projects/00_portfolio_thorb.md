---
title: Thorb
image: '/assets/portfolio_thorb/thorb_thumbnail.jpg'
---
[](/assets/portfolio_thorb/thorb_thumbnail.jpg)

<div style="text-align:center">
    <a href="https://github.com/TheNickOfTime/thorb/releases/download/v1.0/thorb_win64_v1.0.zip" target="_blank" class="button button--primary">Download</a>
    <a href="https://github.com/TheNickOfTime/thorb" target="_blank" class="button button--primary">Source</a>
</div>

<br>

<p><iframe src="https://www.youtube.com/embed/KRncx_Q8qEc" loading="lazy" frameborder="0" allowfullscreen></iframe></p>

# Introduction
Thorb is an FPS "Doom-Like" or "Boomer Shooter" with a bullet-hell minigame thrown in the mix.

This project was created over several months by a group of Naughty Dog QA Members in our free time outside of work - we called this effort the "NDQA Game Chill." The "Game Chill" was conceptualized by myself and [David Flyr](), and then we recruited volunteers from some of our close/trusted coworkers. The goal was to produce a higher quality project, over a longer period of time compared to a game jam. The goal was also to avoid the negative effects one might experience in a game jam - losing sleep, time-crunch stress/anxiety, poor work/life balance, etc.

This was a fantastic experience that allowed everyone that participated to work on a project more substantial than anything we could have made on our own. It did come with some curve balls for us though - namely how to maintain a work/life balance while shipping a AAA game at work. There were also some growing pains for those not experienced using version control, or working in the Unreal Engine. This required me to step into a few different roles that I haven't had to before such as acting as a director of the game, while simultaneously being the "IT" support for everyone on the project.

<div class="gallery-box">
  <div class="gallery">
    <img src="/assets/portfolio_thorb/thorb_screenshot_00.jpg" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_01.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_02.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_03.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_04.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_05.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_06.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_07.png" loading="lazy" alt="Car">
    <img src="/assets/portfolio_thorb/thorb_screenshot_08.png" loading="lazy" alt="Car">
  </div>
</div>

# Highlights
With this being a group project I was very fortunate to not have to work on *every* aspect of the game. So here are some of the systems I did the majority of the work on:

## Player Movement
Movement is such an important aspect of a game like this. Much like doom and games like it, to remain still is to die. So the player is constantly moving, and because of that, movement has to feel good and feel fun.

The player's dash ability is at the core of the movement system. Having an omnidirectional dash movement opens up tons of gameplay opportunities. The player can dash towards things they want to get to more quickly. They can dash out of sticky situations. They can dash upwards (though I clamped how far upwards they can dash) to get to places their jump can't take them. Getting this feeling right and feeling good is an accomplishment I am incredibly proud of. This is also a great moment to thank [Levi Blank]() who designed levels that were worth dashing in.

## Enemy AI
I was initially not going to be responsible for creating the enemy AI, but due to availability of others working on the project I was the next best equipped person to do so. Knowing how important enemies would be to the combat of this game, I was intimidated by what a daunting task this would be. I created a model that I thought was pretty simple: Have a handful of enemies actively pursue the player, and have the rest fall back and lay down suppressive fire to keep the player on their toes. I ended up choosing the 3 closest enemies to chase the player, and have the rest stay put. Because the player is constantly moving, the active enemies constantly change, which means the overall combat scenario is always evolving.

Interestingly, this was one of the last features to make it into the game. Before we had enemies running around, we barely had any idea whether everything in the game would tie well together. Thankfully it did perfectly. I am incredibly pleased with the overall effect the AI has despite being relatively simple. People that played the game often brought it up as a highlight of the game, which was something I never could have anticipated when I started working on this.

## Bullet-Hell Minigame
Originally we were planning on having more than one minigame, but due to many constraints we pulled back the scope and focused on this one. This was a situation where I fulfilled more of a programmer's role than a designers. For this aspect of the game, I built the underlying framework of the bullet hell system, while [Rylan Worker](https://rylanworker.com) created the actual content and various levels of the bullet hell minigame. I was happy that I was able to build a robust enough system that allowed Rylan to create so many unique levels. I think this bullet-hell minigame became a fantastic way to breakup the pacing of our gameplay, and there is no denying that the levels themselves are a significant, yet manageable challenge.

# UI
This was a rare circumstance where I had the privilege of implementing our UI based off of UI mockups designed by [Sami Hagerman](https://samisquared.artstation.com/). It was a great experience since I only had to worry about the functionality of the UI, rather than the artistic vision of it as well. While our UI is not a significant aspect of the game, I think it is perfectly simple and functional while being stylistically consistent with the rest of the game. I am particularly happy we were able to get a working level select menu.

# The Game Chill
Normally the project itself is all I have to talk about, but given I organized the activty that produced this project I have a few more talking points.

## Directing
Aside from telling myself what to do, I've never been put in a directing position while making a game. While we tried to allow as much individual freedom as possible for contributors to this project, we had to organize everyone and occasionally tell people what to do/work on. Additionally from a project management perspective, we had to maintain something of a schedule, and ensure the scope of the game was reasonable. Ultimately it was really important for us to adhere to the mission statement of the project, to maintain the "chill" that we based this concept around. There were several curve balls that made this difficult.

Initially people's individual availability to work on the project would change, but it wouldn't be communicated. Learning to be proactive about communicating with people about their bandwidth was necessary - sometimes even they didn't realize they had too much on their plate till they were approached.

Eventually the pace of working on *The Last of Us: Part I* at work made maintaining a proper work/life balance impossible. Essentially there was no amount of working on this game outside of work that would be healthy for people to do. So we made the hard decision to put the project on hiatus to preserve everyone's mental health - this was the case from approximately June - September of 2022.

Getting the ball rolling after the hiatus was *very* difficult, but I am proud to say I somewhat single handedly initiated that. It was hard, but we put in enough work to wrap this thing up. I learned a lot being in this leadership position, but it is safe to say the difficulties that came with it made achieving our end product even sweeter.

## IT Support
At the outset of this project, I was the most knowledgeable person in regards to using version control. By default it was up to me to lay out the processes and infrastructure that enabled us to effectively collaborate with each other.

Initially we were using Git - its the defacto standard for most software projects these days. However in game development, Perforce reins supreme. We quickly found out why - Git is terrible at managing binary assets, and because we were using Unreal's Blueprint system (which are treated as binary files), we quickly ran into unresolvable merge conflicts.

The solution to this was file locking support - something Git doesn't have (at least by default). Because of the amount of people working on the project, Perforce's free tier was out of the question. After a bit of research, I learned that subversion was our best bet for a free vcs with file locking support. Thankfully I have a bit of home-lab self-hosting experience and was able to spin up an instance of Subversion on my local server, which is what we used for the remainder of the project. Self hosting our vcs came with it's own set of problems - most frighteningly the burden of things working fell upon me. There were times that something wasn't working like it should and I had to fix it on my own despite my relative inexperience working with Subversion.

Ultimately the switch was good. File locking enabled us to work worry-free and the GUI we used (TortoiseGit) was much more accessible to the vcs inexperienced on our team. I later found out that Git has a feature called LFS that enables file locking, but since GitHub limits your LFS storage, we would have had to resort to self hosting anyways since our total project size at one point was ~30GB due to some asset packs our artists imported.