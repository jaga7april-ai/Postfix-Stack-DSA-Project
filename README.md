# Postfix Expression Puzzle

A web app that shows how a **stack** evaluates postfix (reverse Polish) expressions.

**Live demo:** _paste your GitHub Pages link here_

## DSA concept: Stack (LIFO)

In postfix notation the operator comes after its operands, e.g. `3 4 + 2 *` means `(3 + 4) * 2`. A stack evaluates it with one left-to-right pass:

1. Read a token.
2. If it is a number, **push** it.
3. If it is an operator, **pop** two numbers, apply the operator, and **push** the result.
4. At the end, the single item left is the answer.

| Operation | Use in the app | Time |
|-----------|----------------|------|
| `push` | Store a number or a result | O(1) |
| `pop`  | Take operands for an operator | O(1) |
| `peek` | Read the final answer | O(1) |

The whole expression is evaluated in O(n) time.

## Features
- Random puzzles with a check-your-answer box
- Step-by-step stack view with a plain-language explanation of each move
- Run all, restart, and new puzzle buttons
- Load your own expression (numbers with `+ - *`)

## Run it
Open `index.html` in a browser. No install or build step.

## Tech
HTML, CSS, and vanilla JavaScript in a single file.
