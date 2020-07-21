# Pac-Man search
Help Pac-Man navigate different mazes in the most efficient way possible for each case.

## How to use
There are no prerequisites, so there is no need for virtual environments, only python3 and git are needed:

```
git clone https://github.com/azarrias/pacman-search.git
cd pacman-search/src
```

From there you can run a great variety of commands, which look like:

```
python pacman.py 
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic 
```

A visualization of the solution that the AI agent has calculated will be provided upon running these commands.
At the end of this visualization, a summary of insightful information will be provided to the user on the terminal.
This information can be used to benchamark different agents, algorithms and heuristics.

For a full list of arguments that you can provide to the pacman.py script, you can run:

```
python pacman.py --help
```

Code for the different search agents and heuristics is in the searchAgents.py script.
On the other hand, search algorithms (DFS, BFS, UCS, A-star, etc) are coded in the search.py script.
