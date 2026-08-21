## Handgman Functional Specifications

#### 1. **Overview**
The Hangman game is a classic word-guessing game where players try to guess a hidden word by suggesting letters within a certain number of attempts. The game will be developed to include both single-player and multiplayer modes(Iteration 2), with features for tracking game history and resuming unfinished games.

#### 2. **Game Modes**

##### 2.1 **Single-Player Mode**
- **Objective**: The player guesses a word chosen randomly from a selected category.
- **Categories**: The game will feature several categories of words (e.g., Animals, Countries, Movies, etc.). The player can select a category before starting the game.
- **Word Selection**: A word will be randomly selected from the chosen category.
- **Hints**: The game will automatically display the first and last letters of the word as hints.
- **Gameplay**:
  - The player guesses one letter at a time.
  - Correct guesses reveal the letter's position(s) in the word.
  - Incorrect guesses add a part to the hangman (e.g., head, body, arms, legs).
  - The game ends when the player either guesses the word correctly or the hangman is fully drawn.

##### 2.2 **Multiplayer Mode** (Iteration 2)
- **Objective**: One player types a word, and the other player attempts to guess it.
- **Word Entry**: 
  - Player 1 enters a word manually.
  - The game will automatically provide the first and last letters as hints to Player 2.
- **Gameplay**:
  - Player 2 guesses one letter at a time.
  - The rest of the game mechanics (e.g., correct/incorrect guesses) follow the same rules as the single-player mode.
- **Game Completion**:
  - The game ends when Player 2 either guesses the word correctly or the hangman is fully drawn.
  - Players can view the result after the game ends.

#### 3. **Game History**
- **History List**: 
  - A history list will keep track of all outgoing (in-progress and completed) games.
  - Each entry will include details such as game mode (single-player or multiplayer), word category, the word itself, date, and game status (ongoing/completed).
- **Resume Functionality**:
  - Players can resume any ongoing game from the history list.
  - If a game is completed, it cannot be resumed. Players can only view the result.
  - For completed games, the result displayed includes the word, number of attempts used, and whether the word was guessed correctly or the hangman was fully drawn.

#### 4. **User Interface**
- **Main Menu**:
  - Options to start a new game (single-player or multiplayer), view game history, and resume a game.
- **Single-Player Game Screen**:
  - Category selection.
  - Display area for the word with first and last letters revealed.
  - Input box for guessing letters.
  - Hangman drawing area.
  - Display for remaining attempts and guessed letters.
- **Multiplayer Game Screen**:
  - Word input field for Player 1.
  - Display area for the word (with first and last letters revealed) for Player 2.
  - Input box for guessing letters.
  - Hangman drawing area.
  - Display for remaining attempts and guessed letters.
- **History Screen**:
  - List of previous games with details and status.
  - Option to resume ongoing games or view the results of completed games.

#### 5. **Game Logic**

##### 5.1 **Word Hints**
- The game automatically displays the first and last letters of the word at the beginning of each game.
- These hints remain visible throughout the game.

##### 5.2 **Guesses and Attempts**
- Players have a limited number of incorrect guesses before the game ends (typically 6-8, configurable).
- Correct guesses reveal all instances of the letter in the word.
- Incorrect guesses add a part to the hangman drawing.

##### 5.3 **Winning and Losing**
- **Winning Condition**: The player wins if they correctly guess all the letters in the word before the hangman is fully drawn.
- **Losing Condition**: The player loses if they use up all their incorrect guesses and the hangman is fully drawn.

#### 6. **Persistence**
- The game will save the state of ongoing games to allow players to resume them later.
- Completed games are stored in history and can be reviewed but not resumed.
