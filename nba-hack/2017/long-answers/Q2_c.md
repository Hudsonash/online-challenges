## Question 2\(c\)
The question is seen below:
>How do you propose to present a solution to the team? You want to ensure the team understands that there is a relatively wide distribution of possible outcomes. What is the solution?

A proposed solution should be brief and include the problem being faced, a clear example of the problem, and the solution to the finance team.

The problem of predicting the gate revenue of the playoffs is the number of possible outcomes and the difference in gate revenue between teams. For example, East2 vs. East7 make $3.50 million in a four game sweep while East4 and East5 make $18.27 million in seven.

To demonstrate the large variation in potential, the playoffs were simulated 1000 times (view simmed_playoffs.csv for the full results).  The total playoff revenue earned for 100 playoffs is seen in Appendix A.  It shows that in 100 examples, the maximum earnings is $301 million while the minimum is $160 million, nearly half the total earnings.

The wide probability distribution can also be seen in the The conference winning teams.  Appendix B contains a table of the number of times each team reached the finals.  While East1 and West1 each make it over half of the time, there are a total of 11 teams who go all the way.  

Lastly, the variability in gate revenue is clearly seen in a histogram (see appendix C for the histogram).  There are three clear peaks, due to the success of teams 1 and 2.  The variability of simulated gate revenue is exceptionally clear, as there is a standard deviation of $25.12 million. This is an extremely wide dispersion.

```
mean: $258.43 million
std dev: $25.12 million
```

The proposed solution to predicting future playoff revenue is to calculate the estimated gate revenue for each round and re-evaluate the estimations.  This allows the finance team to have an updated estimate of the expected gate revenue with each round, and doesn't let large differences from potential first round results skew the expected results of future rounds.  

In the playoff simulation, it prints the expected result of each round.  In addition, the expected value of the total gate revenue is calculated below, which is significantly more accurate than the estimated value of the gate revenue of the entire playoffs.

---
Hudson Ash | Alex Robson | Others  
July 22, 2017
