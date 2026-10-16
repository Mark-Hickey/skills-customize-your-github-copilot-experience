
# 📘 Assignment: Hangman Game

## 🎯 Objective

Build a word-guessing game in Python using strings, loops, conditionals, and user input. Practice tracking a player's progress and ending the game when they win or run out of attempts.

## 📝 Tasks

### 🛠️ Set Up the Hidden Word

#### Description
Create the starting state for a Hangman game by selecting a word and showing the player which letters have been guessed.

#### Requirements
Completed program should:

- Store multiple words in a predefined list and randomly select one
- Display the word as underscores, with spaces between the hidden letters (for example, `_ _ _`)
- Track the letters guessed by the player


### 🛠️ Add Guessing and Game Outcomes

#### Description
Let the player guess letters until they reveal the word or run out of incorrect guesses.

#### Requirements
Completed program should:

- Prompt the player to enter a letter and show the current word progress after each guess
- Track and display how many incorrect guesses remain
- End when the player guesses the word or has no attempts remaining
- Display a message indicating whether the player won or lost
