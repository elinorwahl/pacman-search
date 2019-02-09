# Pac-Man Search

This is a program that trains an AI agent to play the classic arcade game of Pac-Man, developed by [UC Berkeley College](http://ai.berkeley.edu). Its purpose is to demonstrate the use of map-searching algorithms and heuristics - 'heuristic' being a term that simply means a method of solving a problem.

### Description

The parts of the code intended to be filled out by the user are in `search.py` and `searchAgents.py`, in sections marked `"*** YOUR CODE HERE ***"`.

`search.py` contains four different algorithms used by AIs to search simulated spaces:

- Depth-first search, in which a branch of a search tree is chosen and explored branch-by-branch along a sequence of nodes until an end is reached, and the search starts over from the root to follow a new path of branches.

- Breadth-first search, in which all nodes on one level of a search tree are explored before moving along to the nodes on the next level.

- Uniform-cost search, also known as cheapest-first search, in which the cost of taking each branch in the path is calculated, and the possible paths are explored in order from lowest cost to highest.

- A* (A-star) search, in which the path to explore along the search tree is chosen by a calculation that combines the cost of moving to a given node with the cost of moving from that node to the final destination. Like uniform-cost search, this search progresses from the path with the lowest cost to the highest.

`searchAgents.py` defines the Pac-Man agent's goals and search heuristics. The parts of the program intended to be altered by the user are:

- `CornersProblem`, which sets the goal of exploring all four corners of the Pac-Man game space.

- `cornersHeuristic`, which tells the Pac-Man agent how to visit all four corners of the game space by taking the shortest possible route.

- `foodHeuristic`, which tells the Pac-Man agent how to collect food capsules by taking the shortest possible route.

- `AnyFoodSearchProblem`, which sets the goal of finding food capsules.

### Usage

You can run all of the test cases on this code by opening a terminal and executing the command:

    $ python autograder.py

You can also run individual test cases by executing the command (you can replace "q1" with any of the choices q1-q8):

    $ python autograder.py -q q1

To watch a Pac-Man game progress, use the `pacman.py` script to animate the agent searching various domains. You can do this by executing any of the commands in `commands.txt`.
