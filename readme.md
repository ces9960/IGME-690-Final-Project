# IGME 690 Final Project

## Cullen Sullivan

For this project, I wanted to experiment with machine learning in the context of games and simulations.  I used Unity's ml-agents package to create a project where an AI agent attempts to reach a number of randomly-determined points.

The agent navigates by adjusting its velocity to attempt to reach the targets.  After the agent collides with a target, a new target is spawned in a random position.

This project uses reinforcement learning, where the agent is mildly rewarded for successfully colliding with one or more targets, greatly rewarded for colliding with the maximum number of targets, and penalized for going out of bounds.

After 500,000 trials, the trained AI agents manage to hit the first target most of the time, but it's still not uncommon for the agent to go out of bounds.  In comparison, the initial trials were effectively picking a random direction and traveling in that direction until the agent went out of bounds.

As of right now, there is a bug that will require retraining the AI model to properly support moving towards multiple targets in sequence.  As of right now, due to an error that I neglected to fix until after I had already trained the model, the agent only properly seeks the first target before aimlessly wandering until it goes out of bounds.
