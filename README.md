# Tic_Tac_Toe_Problem


Learn the model of your opponents behavior, up to some level of confidence, and then apply dynamic programming to compute an optimal solution given the approximate opponent model. 

Set up a table of numbers, one for each possible state of the game. Each numbers will be the latest estimate of the probability of our winning from that state.

 - Determine an appropriate amount of epochs to train player 1 and 2 winrates
 - Input player position to faciliate playing the game
 - The game is a zero sum game. If both players are playing with an optimal strategy, every game will end in a tie. 

The goal of this problem is to determine a method that would direclty search the space of possible policies for one with the highest probability of winning against an opponent. 

A policy is a rule that tell the player what move to makes for every state of the game. In other words, every possible configuration of Xs and Os on the three-by-three board. 