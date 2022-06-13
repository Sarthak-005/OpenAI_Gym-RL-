# Frozen Lake
Link : https://www.gymlibrary.ml/environments/toy_text/frozen_lake/?highlight=frozen%20lake
<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/58303643/173411638-d7db0149-0e2e-445c-94bd-6ebf334dc975.gif">
</p>
<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/58303643/173411744-2476d6c8-c2a0-407c-a4fc-75628fe14c3a.png">
</p>



Frozen lake involves crossing a frozen lake from Start(S) to Goal(G) without falling into any Holes(H) by walking over the Frozen(F) lake. The agent may not always move in the intended direction due to the slippery nature of the frozen lake.

Action Space
The agent takes a 1-element vector for actions. The action space is (dir), where dir decides direction to move in which can be:

0: LEFT

1: DOWN

2: RIGHT

3: UP

Observation Space
The observation is a value representing the agent’s current position as current_row * nrows + current_col (where both the row and col start at 0). For example, the goal position in the 4x4 map can be calculated as follows: 3 * 4 + 3 = 15. The number of possible observations is dependent on the size of the map. For example, the 4x4 map has 16 possible observations.

Rewards
Reward schedule:

Reach goal(G): +1

Reach hole(H): 0

Reach frozen(F): 0
