# Tic-Tac-toe

This Python program creates a simple Tic Tac Toe game with a graphical user interface (GUI) using the Tkinter library. The game is designed for two players who alternate marking their moves on a 3x3 grid, with "X" and "O" as their respective marks. The game will check for a winner after every move and reset the game once the game ends.

Key Features and Functions:
Main Window Setup:

The Tkinter library is used to create the main window of the game, titled "Tic Tac Toe". This window holds a 3x3 grid of buttons where players can click to place their marks.
Global Variables:

current_player: Keeps track of whose turn it is, initially set to "X".
game_board: A list of size 9 that represents the 3x3 grid. Each index holds either "X", "O", or an empty string ("") to indicate whether a player has placed a mark in that spot.
buttons: A list that holds references to each of the 9 buttons that make up the grid.
Game Flow:

Switch Player: After each move, the switch_player function switches the turn from "X" to "O" and vice versa.

Check for Win: The check_win function checks all possible winning combinations on the board. It verifies whether there are three matching marks (either "X" or "O") in a row, column, or diagonal. If a player wins, it returns the winning player’s mark.

Reset Game: The reset_game function clears the board and resets the game state, including the current player, when the game ends (either due to a win or a draw).

Button Click Event: The button_click function is triggered when a player clicks one of the 9 buttons on the grid. It updates the board with the current player's mark (either "X" or "O"). The game then checks for a winner:

If a player wins, a message is shown announcing the winner, and the game is reset.
If the board is full with no winner (a draw), a draw message is shown, and the game is reset.
If neither condition is met, the turn is passed to the other player by calling switch_player.
Creating Buttons:

A loop is used to create 9 buttons, one for each square in the 3x3 grid. Each button is associated with a button_click function, which is called when a button is pressed. The buttons are arranged in a grid layout using grid() method.
Game End and Reset:

The game automatically resets once a winner is determined or when the game ends in a draw.
Game Flow:
Turn-based gameplay: Players alternate marking "X" and "O" on the grid.
Winning Condition: The first player to get three of their marks in a row (horizontally, vertically, or diagonally) wins.
Draw Condition: If all squares are filled and no player has won, the game ends in a draw.
Game Reset: After the game ends, either due to a win or a draw, the board is reset, and the game can start again.
