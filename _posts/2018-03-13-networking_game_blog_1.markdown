---
layout: post
title:  "Networking Game: Blog Entry 01"
date:   2018-03-13 12:00:00
author: Jamie Hogg
categories: 
- Networking Game Blog
img: 
thumb: 
---

For the final group assignment, we were tasked with making a turn-based game which works over a network. 
This basically meaning having to send packets of data containing the current game session's data to the server and between each client.

After discussion, the game concept came up was a fantasy type game similar to 'Heroes of Might and Magic' in which there are classes such as 
Warrior, Archer, etc on board which can attack enemies and move to other places on the board.

The current idea is to have 5 classes:
- Warrior
- Mage
- Archer
Then the last 2 haven't been decided yet.

It will be a 2-player game in which the players must try to defeat the other player using 5 pawns. These pawns are optional as the player will at start get to choose the classes of each. Example one player could choose all Mages and the other could choose 1 of each class. The players won’t be able to see each other’s class decisions until the game starts so have to also hope they choose classes which 
are effective against the enemy's since we plan to also have class-based damage bonuses against specific classes.

The networking aspect will be the most challenging part which will have to take in the data to server from each player for:
- Which player's turn it is
- when a pawn moves to a new position
- When a pawn attacks
- When a pawn takes damage
- If all the players are connected
- etc

Other Team member's blogs:
- Alex:
  https://stroudie2.github.io/
- Ben:
  https://www.youtube.com/watch?v=qZ86uVLBRv8
- Thomas:
  https://slaeven.github.io/
