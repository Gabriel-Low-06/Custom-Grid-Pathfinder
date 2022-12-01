# Custom-Grid-Pathfinder

Overview: finds the shortest path (allowing up, down, left, & right) from any item on a 2D array to the bottom right corner. Each item on said array has an integer value -- a "path rating" --, and the rating of a given path is the sum of each item on the path. (Sort of like walking down a sidwalk  and adding up the "costs" to step on each sidewalk block.) Inspired by 2021 [advent of code](https://adventofcode.com/2021/day/15). Written in Java.

Advantages: 
1. Speed. Because this is a specific-use-case, it is much faster in that venue than some more generalized algorithims like Djkstra (based on initial tests, to be verified)
2. Easier implementation. Input is just a 2D array of ints.
3. Potentially useful for open-area pathfinding, ie plotting a route on the ocean or through air, where you can visit any adjacent "square".
4. Variable resolution -- in the above example, you could input the "risk level" for every square mile of airspace or every hundred-square miles.

Disadvantages:
1. Specific. Not useful for solving more complex paths. (Tried to generalize, but the resulting algo is so far inefficient).
2. Not thoroughly tested. Bugs may remain.

Future updates:
1. Allowing the end destination to be any square on the grid
2. Further optimization
