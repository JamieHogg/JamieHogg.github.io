---
layout: post
title:  "Snake Game: Blog Entry 02"
date:   2017-10-26 11:00:00
author: Jamie Hogg
categories: 
- Snake Game Blog
img: post02.jpg
thumb: quake_thumb.jpg
---
After spending a very long time trying to get the movement to work in the chosen engine, I have finally managed it.
Currently it is only a green square (because I made a basic green square rather than making a white one and 
then setting the colour in C++ which would've made more sense) which moves up, left, down and right using the arrow keys.
It honestly took me longer than I had hoped to achieve it but figuring out the engine took me a while.
Originally I had tried to do the movement in the 'SnakeGame' class's input function but I firstly felt putting it in 
its own seperate class would be a better option. Also I was originally trying to use booleans rather than the simpler
approach I am currently using.
The sprite with the orignal attempt would not show the movement but just instantly go to the set borders, mainly because I hadn't
called it in the update function though.
Now I am going to focus on getting a new sprite to appear randomly in the area and make a score go up so I can start on the
tail of the snake.
