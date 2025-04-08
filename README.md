# Number Guessing Game

## Project Description
This is a text-based Python game where the player tries to guess a randomly chosen number. The game supports three difficulty levels and provides feedback on whether the guesses are too high or too low. The game keeps track of each round's outcome and saves scores to a file.

## Solution Principle
The game uses Python's standard library to:
- Generate random numbers
- Receive and validate user input
- Persist data to a text file for score tracking

## Project Structure and Functions
The game is divided into modular functions for readability and maintainability:

- **`choose_difficulty()`**: Prompts the user to select a difficulty level. Returns a dictionary with the number range and max attempts.
- **`get_guess(range_max)`**: Gets a valid guess from the player within the defined range.
- **`play_game()`**: Handles the core gameplay loop including guess checking, win/lose logic, and recording the game result.
- **`save_score(target, guesses, success=True)`**: Saves game results to a file called `scores.txt`.
- **`load_scores()`**: Displays previously saved game scores.
- **`main_menu()`**: Provides a menu-based interface to start a game, view scores, or exit.

## Data Structures Used
- **List**: Stores all user guesses in a game round.
- **Dictionary**: Holds difficulty settings (`range` and `max_attempts`) for each difficulty level.

## External Libraries
- Only Python standard libraries are used:
  - `random` for number generation
  - `os` for file existence checks

## Error Handling and Input Validation
- Ensures the user provides valid numeric input
- Validates that guesses are within range
- Catches non-integer inputs to prevent program crashes

## Pair Work
This project was completed individually.
> If done in a pair, mention both contributors and briefly describe who was responsible for what.
