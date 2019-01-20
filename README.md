# Sports Team Optimization : Operation Research

## Introduction:

In Indian Premier League, 11 teams are competing in a round-robin tournament. Before
the tournament, there is an auction to buy players based on the fixed budget for each team, with some limitation on the number of foreign players per team, number of uncapped players per team, etc.
In IPL, the franchise managers have a task of building a good team within the budget
cap. The players are usually selected based on different heuristics, past experiences, or at most some crude methodologies.
Using the player statistics, want to build the best team possible for the lowest cost
possible, using our optimization model.

## Approach:

Each player has multiple parameters based on their role in the game, which determine
the quality of the player. Batsmen have parameters like batting average, strike rate, runs
scored, matches played, number of 4s and 6s, etc. Bowlers have parameters like matches
played; overs bowled, maidens (overs bowled without giving and runs) bowled, wickets are taken, economy, bowling average, etc. Wicketkeepers are usually considered based on the number of catches taken.

### Key performance indicators:
- Batting Performance: It is the sum of the batting averages of the batsmen in the team.
- Bowling Performance: It is the sum of the bowling averages of the bowlers in the team.
- Objective Function: Maximize the difference between batting performance a bowling
performance.

Analysis based on data from 119 IPL players

### Comparison:
We tried to compare our team to last year winner to check how good is our optimization:

#### Last year winner:
2017 Mumbai Indians
We compared our team with Mumbai Indian Tea, with the same budget

|          | Performance Metrics Parameters | MI   | Our Team |
|----------|--------------------------------|------|----------|
| High/low | Budget                         | 2830 | 2830     |
| High     | SR                             | 2249 | 2831     |
| High     | Batting average                | 325  | 460      |
| Low      | BowlerEco                      | 781  | 707      |
| Low      | BowAverage                     | 150  | 107      |

As we can see our new optimized team better regarding numbers. We have high batting score and low bowling score Compared to Mumbai Indian. As we know, Batting parameter should be high, and bowling parameter should be low
