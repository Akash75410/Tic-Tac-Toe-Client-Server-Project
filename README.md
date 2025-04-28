# Tic-Tac-Toe Game (Client-Server)

This is a simple two-player Tic-Tac-Toe game implemented using Python, with a client-server architecture. The game allows two players to play the game interactively over a network. It demonstrates the use of socket programming, threading, and basic game logic.

## Project Overview

- **Client-side**: The client is responsible for connecting to the server, sending user inputs (moves), and displaying the game board and status (such as "your turn," "opponent's turn," "game over," etc.). It uses sockets for communication with the server and handles the game flow and user interface.
  
- **Server-side**: The server manages client connections, organizes the game, and keeps track of the game state. It facilitates the interaction between two players, ensuring that each player alternates turns and enforcing game rules (valid moves, win conditions, etc.).

## Features

- **Client**:
  - Connects to the server and joins the game.
  - Sends player moves to the server.
  - Displays game status (whose turn it is, game result, etc.).
  - Allows a user to play with an opponent in real-time.

- **Server**:
  - Manages player connections and game sessions.
  - Ensures game rules are followed and validates moves.
  - Sends game updates (board state, player turn) to both players.
  - Handles disconnections and ensures smooth gameplay.

## Technologies Used

- **Python**: The entire game is written in Python.
- **Sockets**: Used for client-server communication.
- **Threading**: Used to handle multiple client connections simultaneously.
- **JSON**: Used to structure communication between the client and the server.

## Installation
1. Clone the repository to your local machine:
   git clone https://github.com/yourusername/tic-tac-toe-game.git
   cd tic-tac-toe-game
   
2.Install the required dependencies:
  pip install pygame
  
3.Run the server:
  python server/main.py
  
4.Run the client:
  python client/game.py
  
**##How to Play**
1.Start the server on one machine or terminal.

2.Start the client (here game.py) on two separate machines or terminals (connecting to the server).

3.Enter your nickname when prompted.

4.The game will begin with Player 1 being assigned 'X' and Player 2 being assigned 'O'.

5.Players take turns to place their symbols on the board by entering a number between 0 and 8, which corresponds to the position on the game board (from top-left to bottom-right).

6.The game will notify you when it's your turn, when the opponent's turn is happening, and the final result (win/draw).

**Contributing**
This project is a collaborative effort between:
Akash K (SRN: PES1UG23CS042) - Client-side development
Abhijnan B C (SRN: PES1UG23CS013) - Server-side development

Feel free to fork this repository and contribute!
