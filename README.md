# Sudoku Solvers

A collection of Sudoku solvers written in different programming languages.

All implementations follow the same simple philosophy and use an identical human-readable `.sudoku` file format + CLI workflow. This makes it easy to compare performance, idioms, and developer experience across languages.

> "Why have you written so many Sudoku solvers?"  
> "For fun, and to compare new programming languages as they gain prominence."

## Performance Comparison (54-blank "evil" puzzle)

| Language     | Time (ms) | Status          | Repository |
|--------------|-----------|-----------------|------------|
| Rust         | 11        | ✅ Complete     | [sudoku-solver-rust](https://github.com/maxtremaine/sudoku-solver-rust) |
| Go           | 15        | ✅ Complete     | [sudoku-solver-go](https://github.com/maxtremaine/sudoku-solver-go) |
| Swift        | 60        | ✅ Complete     | [sudoku-solver-swift](https://github.com/maxtremaine/sudoku-solver-swift) |
| TypeScript   | 66        | ✅ Complete     | [sudoku-solver-typescript](https://github.com/maxtremaine/sudoku-solver-typescript) |
| JavaScript   | 74        | ✅ Complete     | [sudoku-solver-javascript](https://github.com/maxtremaine/sudoku-solver-javascript) |
| Python       | 77        | ✅ Complete     | [sudoku-solver-python](https://github.com/maxtremaine/sudoku-solver-python) |
| Pandas       | 1,553     | ✅ Complete     | [solve_with_pandas.py](https://github.com/maxtremaine/sudoku-solver-python/blob/master/solve_with_pandas.py) |
| Elixir       | TBD       | 🚧 In Progress  | [sudoku-solver-elixir](https://github.com/maxtremaine/sudoku-solver-elixir) |
| Zig          | TBD       | 🚧 In Progress  | [sudoku-solver-zig](https://github.com/maxtremaine/sudoku-solver-zig) |

**Note:** All times measured on the same machine using the puzzle in [`puzzles/evil-54-blanks.sudoku`](./puzzles/evil-54-blanks.sudoku).

## Quick Start (Any Solver)

1. Clone the desired language repo
2. Edit `io/start.sudoku` with your puzzle
3. Run the language-specific command included in README.md
4. View the solution in `io/finish.sudoku` and the terminal

## The `.sudoku` File Format

All solvers use the same intuitive, human-readable format.  
Full specification: [docs/format.md](./docs/format.md)

Example:
```text
abc def ghi
1 ___|___|___
2 _3_|1_6|2_7
3 6__|_3_|51_
  -----------
4 32_|__9|___
5 __8|__5|7__
6 ___|8__|_53
  -----------
7 _47|_9_|__8
8 8_1|7_2|_9_
9 ___|___|___
