# CMPLXSY S11 Group 8 Prey-Predator Eco Systems
## Cats vs. Mouse
Our chosen prey-predator eco system is the famous cat vs. mice relationship, wherein the cat acts as the predator and the mouse acts as the prey.

<img src="https://live.staticflickr.com/3266/5726130896_255aa311f7_b.jpg" width="250" >

## Our ecosystem
### User Input
1. Number of Cats 
2. Number of Mice
3. Percentage of Food (probability per cell) - the probability that cheese is present at each cell
4. Show energy - for showing energy labels of the agents
5. Until Tick 500 - for stopping until tick 500. If no, the model stops when there are either no more cats, no more mice, or no more food.

### Agent Behavior (at every tick)
1. Move - Both cats and mice turn randomly to the right and left and then takes a step forward. For every step, **10 energy** is subtracted from the mice and **15 energy** is subtracted from the cat. 
2. Eat - The mice checks the patch they are on. If the patch is **Yellow**, the patch changes to black and the **15 energy** is added to the mouse. On the other hand, the cats check if there is a mouse on the cell they are stepping on. If there is a mouse, the mouse dies and the cat gets **20 energy**.
3. Reproduce - At every tick, both cat and mice can produce 1 offspring at **10%** probability. 
4. Check - At every tick, the energy of all agents are checked. If it is less than or equal to 0, the agent dies.
5. Cheese - At every tick, patches that are black (no cheese) have a **10%** chance for cheese to regrow.
