### Chess Game in C++

This project implements a simple console-based chess game in C++. It supports a basic version of the game with move validation for a few pieces, turn-taking between players, and checkmate detection. The game is designed to run in a console environment and clears the screen after each move to provide a clean display of the chessboard.

### Features

1. **Chessboard Initialization**: Sets up the initial chessboard with pieces in their standard starting positions.
2. **Move Entry**: Allows players to enter their moves in standard chess notation (e.g., `a1 - a6`).
3. **Move Validation**: Validates moves for Rook, Knight, and Bishop pieces to ensure they follow the rules of chess.
4. **Turn-Based Play**: Alternates turns between White and Black players.
5. **Checkmate Detection**: Detects checkmate conditions and announces the winner.
6. **Screen Clearing**: Utilizes the Windows `CLS` command to clear the console screen after each move for a better visual experience.

### Functions and Structure

#### `main` Function
- Initializes the chessboard.
- Manages the main game loop.
- Alternates turns between players.
- Checks for checkmate after each move.

#### `chessboard` Function
- Initializes the chessboard with pieces in their starting positions.
- Uses '.' to represent empty squares.

#### `chessgrid` Function
- Displays the chessboard in the console.
- Shows row and column labels for easy reference.

#### `entermove` Function
- Prompts the player to enter a move.
- Updates the board with the player's move.
- Clears the console screen after each move.

#### `makingmoves` Function
- Validates the player's move.
- Ensures the move is legal for the piece being moved.
- Provides error messages for illegal moves.

#### `checkmate` Function
- Checks if the current player's king is still on the board.
- Determines if the game is in a checkmate state.

### How to Compile and Run

1. **Compile**: Use a C++ compiler to compile the files. For example:
   ```sh
   g++ -o ChessGame main.cpp
   ```
2. **Run**: Execute the compiled program:
   ```sh
   ./ChessGame
   ```

### Future Enhancements

- **Extended Move Validation**: Implement move validation for all chess pieces, including King, Queen, and Pawns.
- **Check Detection**: Add functionality to detect checks and prevent illegal moves that would leave the king in check.
- **Game Save/Load**: Implement the ability to save and load game states.
- **User Interface**: Develop a graphical user interface (GUI) for a more user-friendly experience.
- **AI Opponent**: Add an AI opponent for single-player mode.

This project provides a foundation for a basic chess game in C++, demonstrating core concepts of game development, including board representation, move validation, and turn-based mechanics.
