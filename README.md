# hungry_horse

This repository contains implemetation of several basic RL algorithms such as SARSA, n-step SARSA and Q-Learning. 
The problem is to find a way through a chessboard from bottom-left state to top right state. Only possibilities of movement corresponds to actions of chess horse (Move only in a shape of letter L).

User can define his own chessboard, rewards of step, initial values of states and standard parameters of RL algorithms mentioned above. It is also possible to manually change reward of steps on selected states which are labeled as "deadly states" and marked by red titles.

Detected solution is saved as a set of jpg images into working directory. Bear in mind the algorithm can crash and get stuck in a loop jumping from one state to previous and back again. This situation occurs if parameters of RL algorithm are set poorly. In such a case infinity amount of jpg files will be stored into your pc. I strognly suggest to use debuger for this vizualization.

# Chessboard example
Every step has reward -1. If a horse make a step on the red state the reward is -100. The goal is to find a way from bottom left corner into top right corner with lowest sum of rewards.
![Chessboard](https://github.com/user-attachments/assets/c45374cf-a35e-4463-bf88-166c5a63217a)
