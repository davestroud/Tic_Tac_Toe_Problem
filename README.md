# Tic_Tac_Toe_Problem

Your task is to set up a game of Tic Tac Toe and train a model with a Reinforcment Learning algorithm. After the model is trained, your program shoud allow a user to play the model that you just trained. 

Learn the model of your opponents behavior, up to some level of confidence, and then apply dynamic programming to compute an optimal solution given the approximate opponent model. 

Set up a table of numbers, one for each possible state of the game. Each numbers will be the latest estimate of the probability of our winning from that state.

 - Determine an appropriate amount of epochs to train player 1 and 2 winrates
 - Input player position to faciliate playing the game
 - The game is a zero sum game. If both players are playing with an optimal strategy, every game will end in a tie. 

The goal of this problem is to determine a method that would directly search the space of possible policies for one with the highest probability of winning against an opponent. 

A policy is a rule that tell the player what move to makes for every state of the game. In other words, every possible configuration of Xs and Os on the three-by-three board. 

For each policy considered, an estimate of its winning probability would be obtained by playing some number of games against the opponent. 

## Tic Tac Toe Problem with a Value function
 - Set up a table of numbers, one for each possible state of the game.
  - Each number will be the latest estimate of the states value, and the whole table is the learned value function.
   - 