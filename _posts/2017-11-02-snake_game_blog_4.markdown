---
layout: post
title:  "Snake Game: Blog Entry 04"
date:   2017-09-02 13:35:00
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

<b>What Next?</b><BR>
So this is some of the more difficult parts of a basic version of snake complete, all I really need to do finish the score, make it possible to eat the food and game over when hit the borders. This all will be what I will be working towards next.

