# Gaming-Project---2048
2048 is a single-player game where the player makes actions on a 4 x 4 grid. Initially, there is an empty 4 x 4 grid except two ‘2’ tiles placed on the board randomly. The player moves first, then the computer spawns a ‘2’ tile on an empty grid randomly. When it is the player’s turn, the player will make an action choosing one cardinal direction, ‘sliding’ the entire board in that direction. All non-empty tiles will move towards the edge of the chosen side if able. If two tiles with the same numerical value collide, they will merge and a tile twice the merged value will be spawned. The player wins if a tile with value 2048 is spawned, and loses if no more moves is available.

# Task Definition :
1.State-based Definition 
Player input: Actions (up, down, left and right) based on the current State Computer input: adds a ‘2’ tile on an empty grid randomly based On the current state Output: result state, reward (instant) Terminal state (success): One ‘2048’ tile Terminal state 
(failure): All adjacent tiles occupied and have different values, i.e. no more moves available 


2.Evaluation Metrics 
The main goal of this project is to get a ‘2048’ tile as fast as possible. The success of the system is measured by the state variables, including the number of tiles occupied, tile values, number of moves taken, etc. 

# Infrastructure and Baseline :
In this project, we have chosen an open-source simulator of 2048 written in Anaconda python. The codes are modified to suit our needs. 
Our baseline for this project is a random agent, where a random move of up/down/left/right is chosen at every action step. Comparisons with the baseline are made in the later parts.
