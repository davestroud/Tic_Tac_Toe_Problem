# Tic_Tac_Toe_Problem

## Problem Statement
Your task is to set up a game of Tic Tac Toe and train a model with a Reinforcement Learning algorithm. After the model is trained, your program should allow a user to play the model that you just trained by inputing a position on a Tic Tac Toe board similiar to the one shown below. The goal of this problem is to determine a method that would directly search the space of possible policies for one with the highest probability of winning against an opponent.  

## Sample human interface of Tic Tac Toe game
### input a number to put a chessman
### | q | w | e |
### | a | s | d |
### | z | x | c |

## Requirements
 - Determine an appropriate amount of epochs to train player 1 and 2 winrates
 - Input player position to faciliate playing the game
 - The game is a zero sum game. If both players are playing with an optimal strategy, every game will end in a tie. 
 - Your Epoch's should have a winrate for player 1 and 2
 - Learn the model of your opponents behavior, up to some level of confidence, and then apply dynamic programming to compute an optimal solution given the approximate opponent model. 
 - Set up a table of numbers, one for each possible state of the game. Each numbers will be the latest estimate of the probability of our winning from that state.

 
## Tic Tac Toe Problem with a Value function
 - Set up a table of numbers, one for each possible state of the game.
 - Each number will be the latest estimate of the states value, and the whole table is the learned value function.
 - State A has a higher value than State B, or is considered "better than state B, if the current estimate of the probablity of our winning from A is higher than it is from B. 
 - A policy is a rule that tell the player what move to makes for every state of the game. In other words, every possible configuration of Xs and Os on the three-by-three board. 
 - For each policy considered, an estimate of its winning probability would be obtained by playing some number of games against the opponent.
