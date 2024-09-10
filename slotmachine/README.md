# Slot Machine Game

## Overview
This is a simple slot machine game implemented in JavaScript using ES6 functions. The player deposits money, chooses the number of lines to bet on, places a bet, and spins the slot machine. The goal is to match symbols on the same line to win money based on the symbol's value.

## How the Game Works
1. **Deposit Money**: Players must first deposit money to play.
2. **Choose Number of Lines**: Players can choose how many lines to bet on (1-3).
3. **Place Bet**: Players place a bet for each line they are betting on.
4. **Spin the Slot Machine**: The machine generates random symbols across 3 rows and 3 columns.
5. **Check for Wins**: If all symbols on a line match, the player wins an amount based on the symbol's value.
6. **Repeat or Quit**: Players can choose to play again or quit when they run out of money.

## Game Rules
- Symbols include **A**, **B**, **C**, and **D**, each with a different probability of appearing and different payout values:
  - **A**: Appears 2 times, payout is 5x the bet.
  - **B**: Appears 4 times, payout is 4x the bet.
  - **C**: Appears 6 times, payout is 3x the bet.
  - **D**: Appears 8 times, payout is 2x the bet.
  
- A win is determined when all symbols on a selected line are the same.

## Installation
1. Clone the repository.
2. Install dependencies using npm:
   ```bash
   npm install prompt-sync
   ```
3. Run the game:
   ```bash
   node slotMachine.js
   ```

## Functions

- **deposit**: Prompts the player to deposit an amount of money.
- **getNumberOfLines**: Asks the player to input the number of lines they wish to bet on.
- **getBet**: Prompts the player to enter their bet per line.
- **spin**: Randomly generates the symbols on the slot machine reels.
- **transpose**: Transforms the columns of the slot machine to rows for easy comparison.
- **printRows**: Displays the rows of symbols on the console.
- **getWinnings**: Checks for matching symbols on a line and calculates the total winnings.
- **game**: Runs the main game loop where players can keep playing until they run out of money.

## Example Gameplay
```
Enter a deposit amount: 100
You have a balance of $100
Enter the number of lines to bet on (1-3): 3
Enter the bet per line: 10
C | B | A
A | D | C
D | A | D
You won, $0
Do you want to play again? (y/n)? y
```

## License
This project is open-source and free to use.