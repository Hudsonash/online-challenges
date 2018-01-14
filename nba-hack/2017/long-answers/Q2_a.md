## Question 2(a)

Question 2(a) asks for the probability of a series going to 4, 5, 6, or 7 games.  The full question is seen below:
>As a primer, let’s think about an individual series. Team East1 plays Team East8 in the First Round. Suppose the probability that East1 defeats East8 at home (8 @ 1) is p_H, and the probability that East1 defeats East8 on the road (1 @ 8) is p_A. In terms of p_H and p_A, what is the probability that the series goes exactly N games for N in {4,5,6,7}, regardless of winner? Please give closed-form analytical solutions.

## Answer
The probability that the first round series between East1 and East8 goes to n games is seen below:
```
Probability of winning in 4 games: 84.8751%
Probability of winning in 5 games: 13.9567%
Probability of winning in 6 games: 1.0671%
Probability of winning in 7 games: 0.1011%
Total: 1.0000
```

The probability of a series going to N games are calculated using binomial distributions for a team winning games at home and on the road.  

For example, for a series to last 4 games, the home or away team need to sweep the series. 2 wins must occur at home and 2 wins away. Using the probabilities given in the question's example, the probability of the
```
Distribution:
binom(successes, observations, prob_of_success)

Home team sweep:
binom(2, 2, .978) * binom(2, 2, .942) = 84.875%
   ** probability of winning 2 of 2 at home times winning 2 for 2 away

Away team sweep:
binom(2, 2, 1 - .978) * binom(2, 2, 1 - .942) = 0.0002%
```

The probability of winning five games have the following possibilities:
| G1 (H)| G2 (H) | G3 (A) | G4 (A) | G5 (H) | Distribution |
| :--- | :--- | :--- | :--- | :--- | :--- |
| L | W | W | W | W | 2/3 at home, 2/2 away |
| W | L | W | W | W | 2/3 at home, 2/2 away |
| W | W | L | W | W | 3/3 at home, 1/2 away |
| W | W | W | L | W | 3/3 at home, 1/2 away |

Here, the binomial distributions for the home team are:
```
Home team wins 3 at home, 1 away:
binom(3, 3, h_win) * binom(1, 2, a_win) * binom (1, 2, 1-a_win)
   ** last binomial distribution is the probability the away team wins

Home team wins 2 at home, 2 away:
binom(2, 3, h_win) * binom(2, 2, a_win) * binom (1, 3, 1-h_win)
```

The same distribution occurs for the away team winning in five games with (1 - h_win or a_win) as the probability of success.

The same pattern continues for games 6 and 7, resulting in the above probabilities.

---
Hudson Ash | Alex Robson | Others  
July 22, 2017
