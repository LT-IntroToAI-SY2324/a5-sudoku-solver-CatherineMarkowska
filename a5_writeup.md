# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
The performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles because, for the second/harder board, it took DFS 337 iterations to solve compared to BFS's 556 iterations for a completed board. In Sudoku, DFS might be preferable over the other because it is more efficient and has better performance regardless of the numbers already on the board. However, for the simpler boards, both DFS and BFS had the same amount of iterations.


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
The choice of data structures impacted the implementation and functionality of the algorithms because even though the setup of both data structures was the same, their efficiency was different -- with DFS being much faster than BFS. Alernative data structures or design patterns that could have been used to achieve the same objectives could be a database. When there is a board, the program checks the database for the same board (as there is a large, albeit not infinite number of numbers that could go in each number slot) that then copies the matching board and presents the completed board. 


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
The Sudoku solver might be adapted or extended for larger puzzles or different types of grid-based logic games by having the same ideas of BFS and DFS apply. By changing the paramaters of the board/game and what DFS/BFS are intended to solve, both DFS and BFS can be used for different problems. The lessons learned from this assignment can be applied to real-world problem solving or optimization challenges through the principles of efficiency. As stated before, DFS was faster than BFS for harder problems, which means that DFS is optimized better. Thus, the usage of DFS allows for options to be eliminated more quickly, especially with real-word problems that have a lot of data (for example, DFS could be used when assigning class periods to students to avoid two class periods being assigned for the same period).

