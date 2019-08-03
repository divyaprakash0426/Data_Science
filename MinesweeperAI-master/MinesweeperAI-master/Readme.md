# MineSweeper AI

The representation is a 2D array of squares, with each square storing several fields. For each cell we have the following information:

* status = False Check if a specific cell has a mine or not.
* isVisited = False Check if a cell is opened or not.
* flagged = False Is the cell marked or not?.
* visible= "-" Initially all cells are blocked.
* value = 0 The value inside the cells; 1 - 8 provides the clue information
For the neighbours which have mines or 9 if it is a mine.

Through the program these attributes are going to be updated accordingly and the clue cell information
will be used to determine which cells to be flagged and which one are safe to be opened. Read Project Report for detailed information.

For our implementation, we observed that the algorithm does not have any problem until the size of the
maze is extremely large. It can solve 50x50 minesweeper maze with low mine density(10% mines). After
50x50, the computer runs out of memory or the system crashes. This is a problem-specific constraint as
the Minesweeper problem is an NP-Complete problem. As the dimensions of the maze increases, the
memory requirement will increase exponentially.
The problem that the algorithm faces is where it has to guess between two choices which have equal
probability of being a mine. This is an implementation specific constraint as there will always be such
scenarios where the algorithm will have to make a guess.

#### Read Project Report.pdf file for detailed information.
