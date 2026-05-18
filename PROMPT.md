# Squarelight App Prompt

Create a complete original board game app for exactly 2 players.

The game is called Squarelight. It is inspired by tic tac toe-style point placement, but played on a larger grid of points. Two players, Blue and Red, take turns placing one point of their color on an empty intersection.

## Core Rules

- The game is designed for exactly 2 players.
- Player colors are Blue and Red.
- The app supports Human vs Human and Human vs CPU modes.
- In Human vs CPU mode, the human plays Blue and the CPU plays Red.
- The default board is a 25 x 25 point grid.
- On each turn, the active player places exactly one point on an empty grid point.
- A square is formed by four neighboring corner points.
- A player captures a square only when all four corners of that square are their color.
- When a player captures a square, the square lights up in that player's color.
- The number inside a captured square shows that player's running score at the moment the square was captured.
- Numbers should only appear for captured scoring squares.
- The number must always fit inside the square, even on the large board.
- Capturing one or more squares grants the same player another turn.
- If no square is captured, the turn passes to the other player.
- The player with the most captured squares wins.

## End Game Logic

- The game ends when all points are filled.
- The game should also end early when the winner is mathematically certain.
- After every move, the app should calculate how many remaining uncaptured squares each player could still possibly capture.
- If the trailing player can no longer tie or overtake the leader, the game ends immediately and declares the leader the winner.
- If no remaining square can be captured by either player, the game ends immediately.

## App Requirements

- Build a playable browser app.
- The app should show the board, current player, scores, move count, captured square count, and a play log.
- Include board-size controls.
- Include a game-mode control.
- Include New Game and Undo controls.
- In CPU mode, the CPU should prioritize capturing available squares, blocking the human's immediate captures, and building toward its own future captures.
- The interface should be clean, modern, responsive, and usable on desktop and mobile.
- The game should run as a self-contained static web page with no build step.
