 Assignment 4: TicTacToe Client-Server Game

Overview
A TicTacToe game implementation using Java backend (NanoHTTPD) and React TypeScript frontend.

 Completed Deliverables

1. Instructions Panel 
- Displays "Current Player: X" or "Current Player: O" during gameplay
- Shows " Player X wins!" when someone gets 3 in a row
- Updates dynamically as game state changes

 2. Undo Functionality 
- Undo button reverses the last move
- Uses immutable game state pattern with history tracking
- Works correctly throughout the game

 3. CSS Styling 
- Professional dark navy theme (#1a1a2e, #16213e)
- Red accents (#e94560) for X and borders
- Green accents (#16c784) for playable cells
- Smooth hover effects and animations
- Responsive design for mobile devices

How to Run

 Prerequisites
- Java 17+
- Maven 3.8.7+
- Node.js v24+
- npm

Start Backend Server

cd back-end
mvn exec:exec

Backend runs at: http://localhost:8080

 Start Frontend Server

cd front-end
npm install
npm start

Frontend runs at: http://localhost:3000

Files Modified

Backend (Java)
- back-end/src/main/java/game/Game.java - Added undo() method
- back-end/src/main/java/game/GameState.java - Added currentPlayer and winner fields
- back-end/src/main/java/game/App.java - Added /undo endpoint
Frontend (TypeScript/CSS)
- front-end/src/App.tsx - Added instructions panel and undo button logic
- front-end/src/App.css - Redesigned with dark theme and animations
- front-end/src/game.ts` - Added type definitions for currentPlayer and winner

Testing
- Click cells to place X and O
- Current player changes after each move
- Winner is detected and displayed
- Undo button works correctly
- New Game button resets the board
- Dark theme looks professional

Color Scheme
- Background: Dark navy (#1a1a2e, #16213e)
- Text: Red (#e94560) for X, Green (#16c784) for playable cells
- Borders: Red and green with glow effects
- Accents: Smooth transitions and hover animations

 Author
Malavika Kilaru

Course
CSCI-513-Fall25


