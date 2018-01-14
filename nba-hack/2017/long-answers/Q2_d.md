## Question 2(d)
The full question is seen below:
> d) What is the probability that West1 meets East1 in the Finals? What is the expected total Playoffs gate revenue if West1 meets East1 in the Finals? What if West1 does not meet East1 in the Finals? How does your solution change if – independent of all other series – East5 defeats East4 in the First Round? You don’t know how many games the series went; you just know the outcome.

#### Probability West1 meets East1 in the finals?
The probability of West1 meeting East 1 in the finals is 40.34%.  This is calculated by finding the probability of each possible series of the playoffs and their progression to the finals.  The code is found in nba_sim (attached).

#### Expected Total Playoffs gate revenue if West1 vs East1 occurs
The first round's expected revenue is fixed.  The expected value of the total first round is $87.01 million.

Theoretically, either team in each series can win.  This gives 2^4 possible combinations in each conference.  Since each top seed is guaranteed to move on, this results in eight potential combinations in round 2, where the expected gate revenue is weighted to the percentage of the semi-final matchups occurring.  

The expected revenue of round 2 with the top seeds winning is $60.45 million.  The expected revenue of the third round (containing 1 vs. x) is $80.51 million.  

The finals between East1 and West1 are expected to earn $48.87 million.  

The total expected revenue if east1 plays west1 in the finals is $276.91 million.


#### What if West1 does not meet East1 in the Finals?
All potential playoff outcomes must be considered to determine a total playoff expected value.  Upon weighting each potential series' expected gate revenue given their probability of occurring, we found that the playoffs are expected to generate $258,512,961.34





#### How does your solution change if East5 defeats East4 in the First Round?
If East5 defeats East4, the expected gate revenue for the rest of the playoff decreases.  Previously, there were 16 (2^4) potential semi-final matchups in the East.  With a guaranteed from East5, the expected gate revenue of round two is calculated from eight possibilities.  In addition, all the expected gate revenue will be smaller than if East4 moved through.  The playoff's expected revenue becomes $
