# CubeStructurer

CubeStructurer is an open-source and advanced Rubik's Cube [explorer](#what-is-this) written in C#.

## What is this?

A Rubik's Cube explorer is a program that allows you to find algorithms, solve a cube, run patterns on different scrambles, and more.
CubeStructurer is essentially a more advanced version of [CubeExplorer](https://kociemba.org/download.htm).

## What is this for?

This program is made for the ones that want to optimize their times as much as possible, people who want to make their own methiods, and people who like messing around with the Rubik's Cube.

## How to use
<details>
<summary>Click to expand</summary>

The program has different sections:

1. The saved patterns: Allows you to optimize and run patterns you saved.
2. The virtual cube: A 3D representation of the Rubik's Cube.
3. The command bar: This is a very complicated thing, [so I'll explain it later](#command-bar).

### Command bar

The command bar is the most complicated part of the program.

If you run an algorithm (e.g. R U R' U'), and press enter, it will run the algorithm on the virtual cube.

There are also **commands** starting with a `:`, `/` or whatever key you set in the settings.

#### Commands

---

| Command               | Description                           |
| --------------------- | ------------------------------------- |
| `ptr (pattern, name)` | Adds a pattern to the saved patterns. |
| `opt (pattern, name)`  | Optimizes a pattern.                  |
| `try (pattern, number of scrambles)` | Runs a pattern on a number of scrambles. |
| `run (pattern, name)`  | Runs a pattern on the virtual cube.  |
| `mkalg (complex-ptr, name)` | Creates a pattern from a [complex pattern](#complex-patterns). |
| `del (pattern, name)`  | Deletes a pattern.    |
| `sfile (filename)`     | Saves a file. |
| `lfile (filename)`     | Loads a file. |
| `mrgfile (filename)`   | Merges a file. |
| `vr (var-name, value)` | Sets or makes a variable. |
| `cl`                   | Clears the screen. |

---

#### Complex patterns

Complex patterns **describe something**, **instead of a series of moves**.

For example, a complex pattern could be: `swap (fc(yll).topc, fc(grr).topc)`, this pattern swaps the top corners of the green and yellow faces.

Complex patterns are made of **commands**, **variables**, and **operators**.

While patterns are just moves.

###### Complex patterns commands

| Command               | Description                           |
| --------------------- | ------------------------------------- |
| `swap (a, b)`         | Swaps the positions of pieces.        |
| `rot (a, b)`          | Rotates the pieces.                   |
| `mv(a, pos)`          | Moves the piece to a position.        |
| `lock (a)`            | Makes the piece un-movable.           |
| `unlock (a)`          | Makes the piece movable again.        |

</details>

## About

CubeStructurer is under the public domain.

> Summary of the license: You can do whatever you want with this program, but I am not responsible for anything that happens to you.

## Credits

Note: This project is made just by me.

- Herbert Kociemba for creating CubeExplorer: A project that I heavily based this project on.
- The Microsoft team for creating .NET, C# and Visual Studio (the things I use to make this project).

---

**I hope you enjoy using this project!**
