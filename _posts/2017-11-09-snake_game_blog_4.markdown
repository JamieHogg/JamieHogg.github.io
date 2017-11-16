---
layout: post
title:  "Snake Game: Blog Entry 04"
date:   2017-11-09 15:00:00
author: Jamie Hogg
categories: 
- Snake Game Blog
img: post04.jpg
thumb: snake_thumb.jpg
---
This post is from after the submission so the game was complete atleast to the point of being able to submit it. So a lot has happened since my last post.

<b>Score & Health</b><BR>
So the first thing to talk about is the score, I had originally managed to get it to print but that's all, I couldn't get it to show the updated score. I ended up working out that it was because I was trying to make the renderer print an integer which it really didn't want to do. In the end I had to update the score constanlty along with convert it to a string to get it to print.
I also added a player health into the game. This I felt added more challenge to the game and made it more fun. To put it simply the player starts with 200 health, then each frame the player loses 1 health. If the player ever reached 0 health they'd game over so to stop this would have to collect blue pick-ups constantly which would reset the health to maximum.
This was honestly a last minute addition so wasn't bug free but worked mostly as hoped.

<b>Scene Changing</b><BR>
Since the game starts off at a main menu, I decided making it possible to change scenes was necessary. So I made a Main Menu, Game, Settings and Game Over scene. I couldn't figure out how to make it change via clicking on text so just decided to do it via key inputs to simplify everything. I'm confident I didn't do the scene changing properly as I believe I'm just rendering each sprite over each other to make the effect of the scene changing as I couldn't work out how else to do it. I probably should've made the objects not being used be deleted when not in use but couldn't work out how to do it.

<b>What Next?</b><BR>
Now I just have to wait until friday then see what James thinks of my snake game and hope that it is good enough to pass.

