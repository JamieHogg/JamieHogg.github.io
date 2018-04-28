---
layout: post
title:  "Birdman Game: Blog Entry 02"
date:   2018-03-07 12:00:00
author: Jamie Hogg
categories: 
- Birdman Blog
img: birdman_post.png
thumb: birdman_thumb.jpg
---
After completing the game and getting it marked, it was met with mostly positive feedback, the main negative being 
that it was a bit short. 

<B>Main Things Added</B><BR>
One of the important things added was how the data for each item and object was gained and set. For example, the door 
in the very first scene, there is a text document holding the texture, the text which will appear when nearby it and 
the position of where the sprite is. So, on start-up, this text file is read and used to set all these details. It makes edit positions easier as anyone editing the code doesn't have to look through the code but instead just for the text file containing the data instead.

Scene changes were also added. Due to how we wanted to make the game, having one scene wouldn't work and so we made it so, you could click on arrows to the sides of the window to switch scenes. It was done by simply having an Enum containing scenes then only rendering the sprites for the current scene that is playing by setting the current scene on each arrow button click.

```C++
enum Scenes
{
	ALLEYWAY,
	ALLEYWAY2,
	SMLSTREET,
	TSQUARE,
	DINER,
	THEATER
};
```
Some sprites were also added which were 90% done by myself in an 8-bit style due to it being easier to design in.

<B>What I had Wished We’d Implemented</B><BR>
The game worked very well but did suffer from being a bit short which was pointed out. As in the Enum above, it suggests there were more scenes intended such as the diner and times square. A rooftop area was also planned but fell through due to running out of time.

