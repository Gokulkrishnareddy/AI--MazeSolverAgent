
# AI Maze Solver Agent (Search Algorithms) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)


## Contributors 

* Hrithik Reddy RA2111047010210
* Sai Teja RA2111047010244
* Gokul Krushna RA2111047010190

## Description 

* This project uses Breadth First Search (BFS), Depth First Search (DFS) and A * Search (AS) search methods in order to solve nxn mazes. The code begins by reading in map.txt and assigning its values to an equivalent size 2D array. It then goes through BFS, DFS and AS in order to find exits marked E1, E2 and navigate from bottom left corner to the top right corner of the maze.

* The code makes use of the Deque STL container so that it can be used as a queue for BFS, a stack for DFS and a priority queue for AS. The heuristic function used for AS is the manhattan distance from the current position of the agent to the ending position of the maze.

* The maze is explored by adding FREE nodes surrounding the agent to the open queue. Once these nodes reach the top of the queue, they are popped off and the process is repeated using the popped node. Popped nodes are added to the closed queue in order to let the agent find the path it completed once it reaches the end of the maze. The agent finishes its exploration when it reaches an exit state or there are no nodes left in the open queue, meaning that there is no solution.
