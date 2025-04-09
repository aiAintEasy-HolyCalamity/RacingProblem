# RacingProblem

A robot car wants to travel far, quickly. Three states: Cool, Warm, Overheated Two actions: Slow, Fast Going Fast gives double reward but risks overheating.

Transition Rules: From Cool:

Slow: Stay Cool (+1 point)
Fast: Move to Warm (+2 points)
From Warm:

Slow: 50% chance to Cool (+1), 50% stay Warm (+1)
Fast: 100% chance to Overheat (-10)
From Overheated:

Terminal State (Episode Ends)
Reward Logic:

Slow = +1, Fast = +2 (if possible)
Overheating = -10
This example demonstrates how RL uses Markov Decision Processes (MDP) to balance reward vs risk.
