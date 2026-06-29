# Reversi (Othello) — Game AI

A Java implementation of the board game **Reversi / Othello**, featuring an AI
opponent powered by the **Minimax** algorithm with a heuristic evaluation function.

This was an academic project for the *Artificial Intelligence* course at the
Athens University of Economics and Business (AUEB).

## Features

- Full Reversi/Othello game logic on an 8×8 board (legal moves, captures, end-of-game detection).
- AI opponent using the **Minimax** search algorithm with a **heuristic evaluation function**.
- **Configurable search depth** — the player sets the maximum Minimax depth at startup.
- Two game modes:
  - **Human vs AI** — the player chooses to play first or second and enters moves by row/column.
  - **AI vs AI** — both moves are computed by the heuristic; the first player (X or O) is chosen at random.

## How to run

The game runs from the command line.

```bash
javac *.java
java Main
```

At startup the program asks for:

1. The number of human players:
   - `0` — the computer plays both sides (AI vs AI).
   - `1` — the user plays; you then choose whether to move first or second.
2. The maximum **Minimax depth**.

If you are playing, you enter your move as a board position (row and column).

## Project structure

```
Main.java          Entry point and game loop
Board.java         Board state and move logic
GamePlayer.java    Player / AI move selection (Minimax + heuristic)
Move.java          Representation of a single move
```

## Tech stack

- Java
- Minimax algorithm with heuristic search

## Notes

Academic group project.
