# Bagels_Game
# Jack Compiler and VM Emulator: Bagels Game Project

This project provides a Jack program for a simple guessing game called **Bagels**. In this game, the computer generates a secret three-digit number, and the player attempts to guess it in 20 or fewer tries. After each guess, the computer gives clues to guide the player. A clue of "Fermi" means a digit is correct and in the right position, "Pico" means a digit is correct but in the wrong position, and "Bagels" means no digits are correct.

## Getting Started

To run this project, you will need the Jack compiler and VM emulator. You can run the game in two ways:

### Online:
Use the Jack compiler on the [Nand2Tetris Web IDE](https://nand2tetris.github.io/web-ide/chip/).

### Locally:
Download the [Nand2Tetris software suite](https://drive.google.com/file/d/1IkIR8Pwq3PY49QgXpUJOkUUVht-TKIET/view) from the official link and run the compiler and emulator on your machine.

## Compiling and Running the Program

### Set Up Program Files
1. Create a new folder to hold the program files (e.g., `BagelsGame`).
2. Download and place the following files in this folder:
   - `Main.jack`
   - `MoreMath.jack`

### Write and Compile the Program
1. Write or modify the Jack program by editing the `.jack` files.
2. Compile the program folder using the Jack compiler to translate all `.jack` files into corresponding `.vm` files.
3. Fix any compilation errors reported, then recompile.

### Run the Program in the VM Emulator
1. Load the compiled `.vm` files into the VM emulator.
2. Run the game and debug if necessary. After each change, recompile and re-run.

## Program Explanation

### Main.jack
The `Main.jack` file contains the primary logic for the Bagels game. Key components include:
- **User Interaction**: Prompts the player to view instructions or start the game directly.
- **Random Number Generation**: Uses the `MoreMath` class to generate a three-digit random number as the secret.
- **Game Loop**: Allows the player up to 20 guesses, with feedback given after each guess:
  - **Fermi**: Correct digit in the correct place.
  - **Pico**: Correct digit in the wrong place.
  - **Bagels**: No correct digits.
- **Guess Evaluation**: Checks if the player’s guess matches the secret number.

### MoreMath.jack
The `MoreMath.jack` file provides helper methods for random number generation:
- **Modulo Operation**: Returns the remainder of a division operation.
- **Random Number Generation**: Uses a linear congruential generator with preselected parameters.
- **Seed Generation**: Obtains a seed based on keyboard timing to initialize the random number sequence.

Together, `Main.jack` and `MoreMath.jack` work to create a fun guessing game with simple feedback messages for the user.

## Running the Game

Follow the steps in **Compiling and Running the Program** above, and you’re ready to play!
