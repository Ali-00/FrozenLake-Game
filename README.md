# FrozenLake-Game
In Frozen Lake environment we teach the agent to move from one block to another and learn from the mistakes.
he Frozen Lake environment is a 4×4 grid which contain four possible areas  — Safe (S), Frozen (F), Hole (H) and Goal (G). The agent moves around the grid until it reaches the goal or the hole. If it falls into the hole, it has to start from the beginning and is rewarded the value 0. The process continues until it learns from every mistake and reaches the goal eventually.
The agent in the environment has four possible moves — Up, Down, Left and Right. One of the Reinforcement Learning techniques, Q-Learning used here. This environment will allow the agent to move accordingly. There could be a random action happening once every a few episodes — let’s say the agent is slipping in different directions because it is hard to walk on a frozen surface. Considering this situation, we need to allow some random movement at first, but eventually try to reduce its probability. This way we can correct the error caused by minimising the loss.

The surface is described using a grid like the following:
SFFF       (S: starting point, safe)
FHFH       (F: frozen surface, safe)
FFFH       (H: hole, fall to your doom)
HFFG       (G: goal, where the frisbee is located)
