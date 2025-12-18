# 02-exploring-simple-cases

## Notation

Let $W_{i}$ be the probability that player $i$ wins the game, $W_{max}$ correspond to the maximum probability out of all the players, and $W$ correspond to the player(s) that has that probability.

Note also that n-uel refers to generalised $n$ player 'duel', with any accuracy probability distribution, while nh-uel refers to an $n$ player 'duel' where the accuracy probability distribution specifcally takes the form specified in the original question (h because it's essentially the harmonic series). These more complicated generalised cases are explored later separately in the project.

## $n=1$

In the case of one player (1h-uel or 1-uel), they will immediately win as they are the only player in the game.

Thus, $W=1$ and $W_{max}=1$.

## $n=2$

In the case of two players (2h-uel), player one's optimal strategy is obviously to fruit player two. They have a probabilty $0.5$ or being succesful and winning the game. If they miss, player two will fruit them with probability $1$.

Thus, $W=1,2$ and $W_{max}=0.5$.

## $n=3$

In the case of three players (3h-uel), player one's optimal strategy is a bit more unclear. A more detailed breakdown of this case is given in 021-n=3.md (add link) where we can see that player one's optimal strategy is in fact to fruit at no one. Player two must then of course fruit player three. If this is successful, the winner is determined by a duel (2-uel) between player one and player two, with player two fruiting first. If this is unsuccessful, player three will fruit player two and the winner will then be determined by a 2-uel between player one and player three, with player one fruiting first. Overall, and perhaps surprisingly, this leads to player one having the greatest chance of winning ($W_{1}=0.4$), player two the second best ($W_{2}=0.38$) and player three the worst ($W_{3}=0.22$).

Thus, $W=1$ and $W_{max}=0.4$.

## Summary Results Table

e.g. n, player prob (1,2,3..), best chance, prob of best chance
