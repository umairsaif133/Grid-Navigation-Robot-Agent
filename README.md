# Grid-Navigation-Robot-Agent
Design and implement an agent that navigates a 4x4 grid world. The agent starts at a random location, and its goal is to reach a fixed destination. Along the way, the agent must be able to sense obstacles which are randomly placed on the grid and make decisions to avoid them.

<img width="603" height="474" alt="image" src="https://github.com/user-attachments/assets/2648f065-5856-4f54-bdd9-7c884fb3762a" />


Algorithm: Grid Agent Navigation

Input: Grid size = 4, random obstacles, goal = (3,3)
Output: Agent path or failure message

Initialize Environment
1.1 Create a 4×4 grid filled with '.'
1.2 Randomly place 4 obstacles ('#'), excluding the goal
1.3 Mark goal cell as 'G'

Set Starting Position
2.1 Randomly choose a start cell not equal to goal or obstacle

Simulation Loop (max 30 steps)
3.1 While agent ≠ goal and steps < 30:
  a. Detect obstacles in four directions (up, down, left, right)
  b. Determine preferred moves toward goal
  c. Remove blocked directions
  d. If no preferred moves, choose any safe direction
  e. If no moves available, stop (agent stuck)
  f. Move agent to new position and increment step count
  g. Print current grid

Check Result
4.1 If agent reached goal → print “Success”
4.2 Else → print “Failed to reach goal”
