---
title: "Is tictactoe solved ?"
date: 2021-02-25
layout: post
permalink: /tictactoe/
---
Tictactoe is probably one of the easiest and earliest games played by humans. Here we try to answer the question: What does an optimal for tictactoe look like , and is there **the** optimal solution ? 

### Tictactoe: Objective and Design
#### Objective:
Tictactoe is a two player game, played on a 3X3 board, where players alternate in choosing one of the nine cells to make their mark. The objective is to get three of your marks in a line, either vertical,horizontal or diagonal. If a player completes the objective, they win, and automatically, the opponent loses, and vice versa. If neither player can complete and the board gets filled, the game ends in a draw.   
I played around and created a simulator that drives the game by accepting actions for both players.
#### Design: 
The two players are denoted as Player 1 and Player 2, with Player 1 making the first move. The game ends with a single score, that takes values from {1, 0, -1} indicating Player 1 wins, Draw and Player 2 wins respectively. This way of scoring allows us to write the objective of the game mathematically, with Player 1 trying to maximize the score, and Player 2 trying to minimize it. For visual representations, consider marks for players 1 and 2 to be 'X' and 'O' respectively, although the simulator uses numbers 1 and 2 to denote the marks of corresponding players. 0 is used to denote empty or unmarked cell.
