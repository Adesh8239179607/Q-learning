# snakegameQ
An automated agent based on the concept of Q-Learning for playing the popular snake game.
## major changes made:
Updated the standard Q-model by replacing one policy network with 2 networks namely the target and policy network and providing a difference in their update frequency for better and more stabilized convergence.

Updated the reward function by introducing penalities for getting trapped in loops and for moving away from the food at any instance in addition to the standard rewards for eating,collision etc.

Tried many function for the change of epsilon for the epsilon greedy strategy like step functions, linears and exponential. Finally settled for exponential due to its asymptotic behaviour which always keeps a chance open for exploration.

Increased the model complexity to 11-(1024)-3 where 11 is the count of state variables and 3 is count of action variables.

## results:
 The model gradually settles at an average score of about 30 with records as high as 80-90+ scores in the setup defined in code.
