---
layout: post
title:  "Networking Game: Blog Entry 02"
date:   2018-04-16 12:00:00
author: Jamie Hogg
categories: 
- Networking Game Blog
img: network_post.png
thumb: network_thumb.jpg
---
Much progress has been made to the actual game itself.

<B>Board</B><BR>
The board now renders in scene once the game starts. The player is able to select their own character which updates the surrounding cells
making them change colour if they are able to move to that location or not. This was able to be done as the board was made by rendering the cells seperately as aposed to instead rendering the board as a whole as its own sprite.

<B>Classes/Characters</B><BR>
As before only 3 out of the total classes had been decided, the last 2 had now been decided. The last 2 classes are:
  - Lancer
  - Assassin

![alt text](https://github.com/JamieHogg/JamieHogg.github.io/tree/master/assets/img/all_sprites.png "Logo Title Text 1")

JamieHogg.github.io/assets/img/
  
The idea for the lancer was for a class similar to the warrior but with more range but lower attack. Then for the assassin to have really high range to be able hit enemies far away by being really agile but to do short amount of damage.

Movement also work for the pawns. So when a pawn is selected and the movable area is shown. If the player clicks on a movable area cell, the selected pawn will move to that location. It also works so the player can only move pawns to a movable cell, plus the movable area updates after movement.

<B>Networking</B><BR>
Not much has progressed with the networking of the game due to the difficulty of the task. Some simple packets have been managed to be
sent but they don't effect the game yet.
  
<B>Things Left to do:</B>
  - Make each team spawn onto their own side of the board
  - Make the right number of pawns spawn on for each team with the correct sprite texture
  - Have the melee and ranged attacks implemented and actually do damage
  - Be able to change the player's pawn classes in the lobby
  - Actually have the game working over the network
  - Have the chat between the 2 players

<B>Other Team member's blogs:</B>
- Alex:
  https://stroudie2.github.io/
- Ben:
  https://www.youtube.com/watch?v=qZ86uVLBRv8
- Thomas:
  https://slaeven.github.io/
