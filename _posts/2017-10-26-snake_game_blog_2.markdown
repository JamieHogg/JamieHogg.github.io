---
layout: post
title:  "Snake Game: Blog Entry 02"
date:   2017-10-26 11:00:00
author: Jamie Hogg
categories: 
- Snake Game Blog
img: post04.jpg
thumb: snake_thumb.jpg
---
So I have finally managed to make progress on the snake game, it took a lot longer than I had expected it to.
This engine is not at all easy to understand and is just as complex as I had originally thought it would be.

<b>Movement</b><BR>
So firstly, I managed to get a square sprite to move around the screen depending on which of the arrow keys had been pressed by the player. This was annoying but way simpler than I originally thought, the only real problem I kept having was getting it to update the position each frame. Originally I had it where the sprite would just teleport to the edges of the border which I had set up. It would do all the incrementing the position but wouldn't display it each frame and instead just put it in the end position. Obviously this was not the desired outcome I had hoped for, in the end I worked out that I had to get it to update in the 'update' function. It took awhile but I ended up getting it to work as planned for now. It currently is moving one space each frame in each direction at the moment which looks nice however I want a more classic style of snake in which it moves the sprite size each time so will attempt to do it later using some kind of delay function possibly.

```C++
switch (key_dir)
	{
		case ASGE::KEYS::KEY_LEFT:
		{
			x--;
			break;
		}
		case ASGE::KEYS::KEY_RIGHT:
		{
			x++;
			break;
		}
		case ASGE::KEYS::KEY_UP:
		{
			y--;
			break;
		}		
		case ASGE::KEYS::KEY_DOWN:
		{
			y++;
			break;
		}
	}
```

This is my simple loop currently which checks for a button being pressed, then checks which one and moves a square sprite around the screen by 1 each frame.

<b>What Next?</b><BR>
The next big thing I feel I should work on is the tail, the biggest reason being that it is most likely going to be the part of the game I most struggle with. I have an idea in which I would store the X and Y positions in 2 separate arrays, it's just how to set the values of each movement which I'm struggling with working out how to do mainly.
