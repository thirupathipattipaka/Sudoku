# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?
A: Naked twins are defined as two squares in the same unit that contains the same numbers eg: A1:23, A2:23. There is certainly cent percent chance that these two numbers will go either A1 or A2 (not sure which number is where) and zero percent chace that these numbers will go into the other squares in the unit. So we can eliminate these numbers from other squares in the unit. These updates to other sqaures in the unit will cause further updates to its peers, and the peers of those peers, and so on. This is how we can solve the Naked twins problem and complete to solve the sudoku problem.
 
# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?
A: In the diagonal sudoku problem, I have just added another constriant such as diagonal units to the unitlists. The nuber of peers are increased for the diagonal squares which will help to add another contraint while solving the sudoku problem. All the remaining constraints and programs are same as the normal sudoku.
### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in function.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
