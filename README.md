# SudokuSolver
# Sudoku Solver

A simple sudoku solver written in Python using backtracking.

## How it works

The solver scans the board for an empty cell, tries numbers 1-9, and checks if
the number is valid in that row, column, and 3x3 box. If valid, it places the
number and recurses. If it gets stuck, it backtracks and tries the next number.

## Usage

Run the script directly:

    python sudoku.py

Edit the `board` variable at the top of the file to use your own puzzle.
Use `0` for empty cells.

## Example output

    Puzzle:

    5 3 . | . 7 . | . . .
    6 . . | 1 9 5 | . . .
    . 9 8 | . . . | . 6 .
    ------+-------+------
    8 . . | . 6 . | . . 3
    4 . . | 8 . 3 | . . 1
    7 . . | . 2 . | . . 6
    ------+-------+------
    . 6 . | . . . | 2 8 .
    . . . | 4 1 9 | . . 5
    . . . | . 8 . | . 7 9

    Solved:

    5 3 4 | 6 7 8 | 9 1 2
    6 7 2 | 1 9 5 | 3 4 8
    1 9 8 | 3 4 2 | 5 6 7
    ------+-------+------
    8 5 9 | 7 6 1 | 4 2 3
    4 2 6 | 8 5 3 | 7 9 1
    7 1 3 | 9 2 4 | 8 5 6
    ------+-------+------
    9 6 1 | 5 3 7 | 2 8 4
    2 8 7 | 4 1 9 | 6 3 5
    3 4 5 | 2 8 6 | 1 7 9

## Requirements

Python 3 - no external libraries needed.
