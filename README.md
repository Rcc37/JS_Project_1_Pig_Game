# JS_Project_1_Dice_game
# Dice Game

This project is a simple two-player **Dice Game** built using **HTML**, **CSS**, and **JavaScript**. It focuses on concepts like DOM manipulation, event handling, and game logic. The players roll a dice to accumulate scores, and the first player to reach a predefined target score wins.

---

## Features

- **Two-player Gameplay**: Alternate turns for players.
- **Dice Roll Mechanism**: Generates a random number between 1 and 6.
- **Switch Player Functionality**: Automatically switches players if the dice rolls a `1`.
- **Hold Functionality**: Allows players to save their current score.
- **Winner Highlighting**: The winner is displayed visually.
- **Game Reset**: A reset button to start a new game.

---

## Technologies Used

- **HTML**: For structuring the webpage.
- **CSS**: For styling the game interface.
- **JavaScript**: For game logic and interactivity.

---

## Project Structure

### **HTML Elements**
- `.player--0` and `.player--1`: Represent the two players.
- `#score--0` and `#score--1`: Display the total scores of Player 1 and Player 2.
- `#current--0` and `#current--1`: Display the current score for each player during their turn.
- `.dice`: The dice image, dynamically updated based on the roll.
- `.btn--new`: Button to reset the game.
- `.btn--roll`: Button to roll the dice.
- `.btn--hold`: Button to hold the current score.

### **JavaScript Logic**

1. **Game Initialization**:
   - `init()` sets the initial state of the game, including resetting scores, hiding the dice, and setting the active player.

2. **Rolling the Dice**:
   - `btnRoll.addEventListener('click', ...)` generates a random number for the dice roll, updates the UI, and checks for a roll of `1`.

3. **Switching Players**:
   - `switchPlayer()` resets the current score and toggles the active player.

4. **Holding Scores**:
   - `btnHold.addEventListener('click', ...)` adds the current score to the active player's total score, checks for a win condition, and switches players if necessary.

5. **Winning Condition**:
   - If a player's score reaches or exceeds 100, the game ends, and the winner is highlighted.

6. **Resetting the Game**:
   - `btnNew.addEventListener('click', init)` resets the game to its initial state.

---

## How to Play

1. Open the game in a web browser.
2. Player 1 starts the game by rolling the dice using the **Roll Dice** button.
3. The player can choose to:
   - Roll the dice again to accumulate more points.
   - Hold their score using the **Hold** button to save their current score and pass the turn to the other player.
4. If the dice rolls a `1`, the current score is reset, and the turn passes to the other player automatically.
5. The first player to reach a score of **100 or more** wins the game.
6. Click the **New Game** button to reset the game.

---

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Open the `index.html` file in your browser.

---

## Potential Improvements

- Add customizable winning scores.
- Implement more player options (e.g., more than 2 players).
- Add animations for dice rolls.
- Include sound effects for better user interaction.
- Make the game responsive for mobile devices.

---

## License

This project is open-source and available under the [MIT License](LICENSE).

---

Enjoy the game and happy coding!


