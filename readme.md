# IGME 690 Final Project

## Cullen Sullivan

For this project, I wanted to experiment with machine learning in the context of games and simulations.  I used Unity's ml-agents package to create a project where an AI agent attempts to reach a number of randomly-determined points.

The agent navigates by adjusting its velocity to attempt to reach the targets.  After the agent collides with a target, the agent's position is reset and a new target is spawned in a random position.

This project uses reinforcement learning, where the agent is mildly rewarded for successfully colliding with one or more targets, greatly rewarded for colliding with the maximum number of targets, and penalized for going out of bounds.
