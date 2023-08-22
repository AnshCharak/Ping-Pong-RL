## Introduction

This repo trains a Reinforcement Learning Neural Network so that it's able to play Pong from raw pixel input.
Based on the [Playing Atari with Deep Reinforcement Learning paper by Mnih et al.](https://arxiv.org/abs/1312.5602)


## The AI Agent Pong in action

### Prior to training (mostly random actions)
![Prior to training (mostly random actions)](https://github.com/omkarv/pong-from-pixels/blob/master/experiment-output/base-init.gif)

### After training base repo + learning rate modification
![After training](https://github.com/omkarv/pong-from-pixels/blob/master/experiment-output/base-after-overnight-train.gif)

The agent that played this game was trained for ~12000 episodes (basically 12000 episodes of 'best-of-21' rounds) over a period of ~ 15 hours, on a Macbook Pro 2018 with 2.6GHz i7 (6 cores).  The running mean score per episode, over the trailing 100 episodes, at the point I stopped training was -5, i.e. the CPU would win each episode 21-16 on average.

**Graph of reward over time - first 10000 episodes of training**
![Reward over time with bugfix](https://github.com/omkarv/pong-from-pixels/blob/master/experiment-output/bugfix-rewards-chart.png)

**Graph of reward over time - 10000 to 15000 episodes of training**

![Reward over time after 10000 episodes](https://github.com/omkarv/pong-from-pixels/blob/master/experiment-output/bugfix-rewards-chart-after-10000.png)


