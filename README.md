# Clingo-solvers

This repository contains NxN-Sudoku, Yosenabe, Minotaur and Elevator game solvers implemented in [`clingo`](https://github.com/potassco/clingo). The report for the final elevator project can be found [here](./docs/asp_elevator.pdf).

## Dependencies

Install `clingo` onto your system, either via your package manager (recommended, if available) or building from [source](https://github.com/potassco/clingo/blob/master/INSTALL.md).

## Usage

Source code for `clingo` solvers are available in the `src` directory. The `init` directory contains test instances of the respective games.

To test the default 9x9 sudoku solver, execute the following:

```shell
$ clingo ./init/init_sudoku.lp ./src/sudoku.lp 0
```

## Troubleshooting

Based on local experiments, all solvers except the Minotaur solver in `mino.lp` and/or `mino_alt.lp` succeeded in Yeti benchmark tests. Pull requests for an improved Minotaur solver are therefore very welcome.

## Vim syntax-highlighting

In order to initialize syntax highlighting for `clingo` in `vim`, simply copy the 3 folders inside this repository's `vim` directory into your local `~/.vim` directory.

Source and further information: https://sourceforge.net/p/potassco/code/HEAD/tree/trunk/vim-syntax-gringo/
