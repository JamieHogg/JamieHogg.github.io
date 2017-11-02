---
layout: post
title:  "Snake Game: Blog Entry 02"
date:   2017-11-02 12:00:00
author: Jamie Hogg
categories: 
- Snake Game Blog
img: post02.jpg
thumb: quake_thumb.jpg
---
Since the last blog post, where I had only just finished/worked out the movement for the snake sprite, I have achieved a lot which also isn't much at all. 

Movement
Firstly, I wanted to make the sprite move a specific number of spaces each time it moved like the classic versions of snake. I also realized that it would just make coding everything excessively easier as the collision can be solved by the head part of the sprite just being equal to the target. Actually making it move the specific number of spaces was the easy part, because I had it set up so that each time I pressed one of the arrow keys, the head sprite of the snake will move 1 space in the chosen direction each frame. Due to the size of the sprite being 25x25 pixels, I needed to change the size the sprite moved to 25 which was easy. 
For example when the player presses the right key, I used the code 'x++', which as I said earlier moves it 1 space, so I changed it to 'x=+25'. This does the desired effect but it moves 25 spaces each frame which is obviously way too fast which isn't what I want.
In order to slow it down I needed to make some kind of delay/wait function, luckily I found one online which I edited to fit my problem.


