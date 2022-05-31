# React Treasure Hunt Game

### Remember:
- Pseudocode!!
- Ask clarifying questions

### User Stories
- As a user, I can see a page with a 3 by 3 grid board game with a question mark in each square.
  - branch: board-creation
  - Rendered a single square with basic css
  - Iterated over the board to create 9 squares using the map method
  - styled board, header and squares to display in 3x3 grid
  - Passed in the value and index through the state
  - Styled question marks
- As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array.
  - new branch: alert-position
  - pass the index to the square component
  - added onclick to square
  - pass method from app to square to get index
- As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji.
  - branch: tree-emoji
  - destructured board from state
  - updated board at index clicked to represent tree emoji
  - updated state to render new tree
  
- As a user, if I select the winning square the question mark will become a treasure emoji and if I select the losing square the question mark will become a bomb emoji.
  - new branch: win-lose
  - created random number for treasure location
  - if treasure clicked money bag emoji will be displayed
  - created click event to change item to bomb

- As a user, I can click on a “Play Again” button that will restart the game.
- As a user, I can see a counter that shows how many guesses I have left. The counter starts at 5 and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).
