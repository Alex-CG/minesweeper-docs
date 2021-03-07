# Action to be performed by the game

[IMPLEMENTED]
* create a new game
* reveal a square
    - when a cell with no adjacent mines is revealed, all adjacent squares will be revealed (and repeat)
    - when a cell with a number is revealed there are more actions to perform
    - when a cell with a mine is revealed the game is over
* flag a square
    - question mark - when you have confirmed that there is a mine
    - red flag - when you suspect that there is a mine
* unflag a square

[PENDING]
* save the progress (set a name to the game for multi game saving support)
* resume the progress (choose from a list of saved games)
