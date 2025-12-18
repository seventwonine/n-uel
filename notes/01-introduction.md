# 01-Introduction

## Formal Definition of Problem

Consider $n$ players, indexed $n_{i}=1, 2, 3... n$, each with an infinite amount of fruit and, on throwing a piece of fruit, probability $p_{i}=\frac{1}{n_{i}}$ of hitting their target. The players take turns throwing fruit at each other, in the ordering of their index numbers, wrapping around from player $n$ to player $1$. When a player is hit by a piece of fruit, they are 'e-lime-anated'. The game continues until there is only one remaining player.

What is the optimal strategy for any given player, and which player has the greatest chance of survival, for a given value of $n$?

## Assumptions

- All players are rational, with their goal being to be the lone survivor.
- No player is hit by a fruit not intended for them.

## Plans for the Project

### Primary Focus

- Theoretically analyse the scenario, with explicit results and probabilities for low $n$, and hopefully generalised formulae and results for all $n$.
- Run computer simulations for the scenario to aid with the above analysis. 

### Other Interesting Cases

- Consider alternate accuracy probability distributions. e.g. an intesting case being for $n=3$, $p_{i}=1$, no one should ever 'fruit' anyone else as they will then immediately be 'fruited' by the remaining player. Therefore the game never ends. This can be remedied by altering the goal of the players to 'fruit' as many other players as possible rather than surviving until the end.
- Consider alternate 'fruiting' orders e.g. for a given number of players can you construct a 'fruiting' order that gives the most balanced survival distribution for all the players.
- Consider whether machine learning methods can be implemented for understanding more complex setups of the scenario

## Inspiration

This project was inspired by the 'Triangular Gunfight' question in Alex Bellos' book 'Can You Solve My Problems?', which focuses specifically on the case $n=3$. This scenario was termed a 'Truel', inspiring the terminology adopted in this project of 'n-uel'. The problem discussed in this project has been reframed in terms of throwing fruit, rather than shooting guns, as that is more 'apple-ealing' (get it). Hence, players are referred to as having been 'fruited' when they are hit and eliminated, and instead of 'shoot' we use 'fruit'.
