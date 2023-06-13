# Description:
The project contains 3 reinforcement learning case studies with 6 algoritms' implementations and comparisons

# FrozenLake & Monte Carlo Control:
Case study concentrates on implementing Monte Carlo Off policy algorithm and further comparison with the On policy algorithm for the FrozenLake game.

The results indicated that in case of 4x4 game grid, the probability of success for MC Off policy was on average 5 percentage points higher. The down direction at the very beginning of the game was the bottleneck for the On policy algorithm. This direction more often was leading to situations where the algorithm was endlessly hitting the upper left corner, where there was a greater chance of slipping and hitting the ice hole. A good choice for the first action plays a big role in this game.

# FrozenLake:
Case study concentrates on implementing brute force algorithm and further comparison with the dynamic programming approach for the FrozenLake game.

- For dynamic programming approach for a 3×3 game grid, the algorithm converged to the optimal solution in 45 iterations (1.32 seconds). 
- In the case of the brute force algorithm, the best solution was found in 262144 iterations (14 minutes 47 seconds).
- The brute force algorithm has a computational complexity of O(4^n2) - therefore, for 4×4 and 8×8 game grids, assuming the same time for 1 iteration, a solution for a 4×4 grid would be found in 115 days. For an 8×8 grid, this is 3.17e+28 years! For comparison, the universe is 13,787e9 (13.787 billion) years old!

# GridWorld:
Case study concentrates on implementing SARSA(lambda) algorithm and further comparison with SARSA(0) for the GridWorld game.

Based on the results, SARSA(lambda =0.5) turned out to be the most effective for the considered GridWorld problem. This is evidenced by the agent's total reward (score), since for lambda=0.5 the number of completed games (episodes) was the largest (729), so as the average episodes before completion (=160). It is worth noting, however, that the obtained results may have been obtained by chance, as the average difference (371-325)/325 = 14.15% is not too large and may result from the random nature of learning.
