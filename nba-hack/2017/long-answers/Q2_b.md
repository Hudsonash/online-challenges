## Question 2(b)
NBA's finance team has forecasted gate revenue and asked for a playoff simulator. The full question is seen below:
> Now suppose that the regular season has just concluded and the NBA playoff picture is set. Team Finance has forecasted gate revenue per game for every team in each possible round – these per-game forecasts for each (team, round) combination are given in the Hypothetical Playoff Gate Data tab in the attached Excel file. Further suppose you are given win_probabilities.csv, which describes the probability that a given team defeats any other team, either at home or on the road. (The format of the probabilities in each row may not be standard.) Note that there is no re-seeding in the NBA Playoffs and that each series follows a 2-2-1-1-1 format. If equal seeds make the Finals, suppose the West team has home court advantage; otherwise, suppose the better seed has home court. Build a playoff simulator that tracks gate revenue using this data. (Assume each game is independent.) Please include any code or any additional materials you used to build your simulator in a zip folder.

The full playoff simulator can be seen at nba_sim.ipynb and attached in the zipped folder.  It simulates a playoff series by simulating each playoff series and summing the total gate revenue of each round.  Here is a sample output of a simulated playoff series given the data presented in win_probabilities and gate_rev:


~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
                          ROUND 1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Series between East1 and East8

(4-0) series win for the home team.
Generated $11.03 million in gate revenue
Expected to generate $11.48 million during the series

Series between East2 and East7

(4-0) series win for the home team.
Generated $2.89 million in gate revenue
Expected to generate $3.39 million during the series

Series between East3 and East6

(4-2) series win for the home team.
Generated $3.85 million in gate revenue
Expected to generate $3.41 million during the series

Series between East4 and East5

(3-4) series loss for the home team.
Generated $22.63 million in gate revenue
Expected to generate $18.67 million during the series

Series between West1 and West8

(4-1) series win for the home team.
Generated $18.12 million in gate revenue
Expected to generate $15.05 million during the series

Series between West2 and West7

(4-0) series win for the home team.
Generated $6.64 million in gate revenue
Expected to generate $7.99 million during the series

Series between West3 and West6

(4-3) series win for the home team.
Generated $19.99 million in gate revenue
Expected to generate $15.43 million during the series

Series between West4 and West5

(3-4) series loss for the home team.
Generated $14.24 million in gate revenue
Expected to generate $11.67 million during the series

Total Gate Revenue Earned to Date: $99.4 million

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
                          ROUND 2
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Series between East1 and East5

(4-2) series win for the home team.
Generated $21.17 million in gate revenue
Expected to generate $18.21 million during the series

Series between East2 and East3

(4-1) series win for the home team.
Generated $4.44 million in gate revenue
Expected to generate $5.07 million during the series

Series between West1 and West5

(4-3) series win for the home team.
Generated $34.5 million in gate revenue
Expected to generate $24.67 million during the series

Series between West2 and West3

(4-2) series win for the home team.
Generated $11.95 million in gate revenue
Expected to generate $11.42 million during the series

Total Gate Revenue Earned to Date: $171.46 million

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
                          ROUND 3
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Series between East1 and East2

(4-1) series win for the home team.
Generated $27.87 million in gate revenue
Expected to generate $32.25 million during the series

Series between West1 and West2

(2-4) series loss for the home team.
Generated $51.46 million in gate revenue
Expected to generate $49.32 million during the series

Total Gate Revenue Earned to Date: $250.79 million

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
                          ROUND 4
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Series between East1 and West2

(4-1) series win for the home team.
Generated $42.09 million in gate revenue
Expected to generate $47.99 million during the series

CHAMPIONS OF THE NBA: East1

TOTAL PLAYOFF REVENUE: $292.882 million.
EXPECTED PLAYOFF REVENUE: $276.016 million.


To run a playoff simulation, import nba_sim and run playoff_sim(display=True).
