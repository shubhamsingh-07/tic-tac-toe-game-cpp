# Tic-Tac-Toe Game in C++

[![Language](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A console-based 3 × 3 Tic-Tac-Toe exercise written in C++. It prints the board, checks rows, columns, and diagonals for a win, and reports a win or draw.

## Features in the Current Code

- Displays the 3 × 3 board and numbered cell instructions.
- Checks winning rows, columns, and both diagonals.
- Ends after a winning pattern or when all nine cells are filled.
- Reports a winner or a draw.

## Important Behavior Note

Although the output labels the sides as **HUMAN** and **COMPUTER**, the current source does not read a player's move from standard input. It shuffles the nine cell positions and automatically assigns those positions to the two sides in sequence. Therefore, the current program is not yet a fully interactive human-versus-computer game.

## Project Structure

```text
tic-tac-toe-game-cpp/
├── tic tac toe game.cpp
├── README.md
└── LICENSE
```

## Compile and Run

This source uses the GNU C++ header `<bits/stdc++.h>` and `std::random_shuffle`, so compile with a GNU-compatible compiler in C++14 mode:

```bash
g++ -std=c++14 "tic tac toe game.cpp" -o tic_tac_toe
./tic_tac_toe
```

On Windows, run the generated executable from the terminal:

```powershell
.\tic_tac_toe.exe
```

## Learning Outcomes

- Two-dimensional arrays and board rendering.
- Functions for initialization, win detection, and result reporting.
- Conditional flow and loops.
- Randomized ordering of cell positions.

## Recommended Improvements

- Add interactive user input and validate that the selected cell is empty.
- Generate computer moves independently from the player's move.
- Replace `random_shuffle` with `std::shuffle` and a random engine.
- Replace `<bits/stdc++.h>` with the standard headers used by the program.
- Add a replay option and automated tests for win/draw detection.

## License

Licensed under the MIT License. See [LICENSE](LICENSE) for details.
