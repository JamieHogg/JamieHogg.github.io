---
layout: post
title:  "Snake Game: Blog Entry 03"
date:   2017-11-02 12:00:00
author: Jamie Hogg
categories: 
- Snake Game Blog
img: post04.jpg
thumb: snake_thumb.jpg
---
Since the last blog post, where I had only just finished/worked out the movement for the snake sprite, I have achieved a lot which also isn't much at all. 

<b>Movement</b><BR>
Firstly, I wanted to make the sprite move a specific number of spaces each time it moved like the classic versions of snake. I also realized that it would just make coding everything excessively easier as the collision can be solved by the head part of the sprite just being equal to the target. Actually making it move the specific number of spaces was the easy part, because I had it set up so that each time I pressed one of the arrow keys, the head sprite of the snake will move 1 space in the chosen direction each frame. Due to the size of the sprite being 25x25 pixels, I needed to change the size the sprite moved to 25 which was easy. 
For example when the player presses the right key, I used the code 'x++', which as I said earlier moves it 1 space, so I changed it to 'x+=25'. This does the desired effect but it moves 25 spaces each frame which is obviously way too fast which isn't what I want.
In order to slow it down I needed to make some kind of delay/wait function, luckily I found one online which I edited to fit my problem.

```C++
void Player::wait(float time)
{
	clock_t endwait;
	endwait = clock() + time * CLOCKS_PER_SEC;
	while (clock() < endwait) {}
}
 ```
 
This function pretty much pauses the game for the chosen time as far as I'm aware. The only real change that I did to the code was that I changed 'time' to float as originally it was an int which didn't work well.

<b>Tail</b><BR>
The next big thing I change/added to the game was the addition of the tail depending on the player score. I haven't managed to get the score working at this current moment in time so am just using a test variable for the score number. For the tail though, I thought it made the most sense to turn the player sprite into an array as making a completely new separate sprite for each tail part would be illogical and take a long time.
So to actually make all the rendering and setting of each sprite part I made 'for' loops around the different parts as the size of the score.
Then I just had to set the positions of each of the tail parts which honestly was difficult for me to figure out. Luckily I found a method of actually setting the values online which I set in arrays of 'tail_x' and 'tail_y'.
	
```C++
int prev_x = tail_x[0];
int prev_y = tail_y[0];
int prev2_x, prev2_y;
tail_x[0] = x;
tail_y[0] = y;

for (int i = 1; i < 100; i++)
{
	prev2_x = tail_x[i];
	prev2_y = tail_y[i];
	tail_x[i] = prev_x;
	tail_y[i] = prev_y;
	prev_x = prev2_x;
	prev_y = prev2_y;
}
```

It's quite confusing but basically each loop it keeps setting each tail part as the position as the part in front of them.

<b>What Next?</b><BR>
So this is some of the more difficult parts of a basic version of snake complete, all I really need to do finish the score, make it possible to eat the food and game over when hit the borders. This all will be what I will be working towards next.

