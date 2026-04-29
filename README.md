# Tic Tac Toe

A clean, browser-based Tic Tac Toe game built with vanilla HTML, CSS, and JavaScript. Two players take turns on the same device — no server, no install required.

---

## Features

- **Two-player local gameplay** — Player X and Player O take turns clicking the board
- **Win detection** — Automatically checks all 8 winning patterns after every move
- **Draw detection** — Declares a draw when all 9 boxes are filled with no winner
- **Live scoreboard** — Tracks wins for both players across multiple rounds, displayed beside the game grid
- **Win overlay** — When someone wins, the board is replaced by a full-screen result message
- **Reset / New Game** — Start a fresh round at any time without losing the score

---

## Project Structure

```
tic-tac-toe/
├── index.html        # Game layout and structure
├── style.css         # Styling and layout
├── app.js            # Game logic (turns, win check, score)
└── backgroundimg.jpg # Background image
```

---

## How to Run

No build tools or dependencies needed.

1. Download or clone the project folder
2. Open `index.html` in any modern browser
3. Start playing

---

## How to Play

1. Player **O** always goes first
2. Click any empty box to place your mark
3. The first player to get **3 in a row** (horizontally, vertically, or diagonally) wins
4. If all 9 boxes are filled with no winner, the game is a **Draw**
5. Click **New Game** on the result screen or **Reset Game** at any time to play again
6. Scores persist until the page is refreshed

---

## Win Patterns

The game checks these 8 combinations after every move:

| Type          | Positions |
| ------------- | --------- |
| Top row       | 0, 1, 2   |
| Middle row    | 3, 4, 5   |
| Bottom row    | 6, 7, 8   |
| Left column   | 0, 3, 6   |
| Middle column | 1, 4, 7   |
| Right column  | 2, 5, 8   |
| Diagonal      | 0, 4, 8   |
| Diagonal      | 2, 4, 6   |

---

## Technologies Used

- **HTML5** — Semantic structure
- **CSS3** — Flexbox layout, transitions, overlay positioning
- **JavaScript (ES6+)** — DOM manipulation, event listeners, game logic

---

## What I Learned Building This

- Querying and manipulating DOM elements with `querySelector`
- Using `forEach` and `for...` loops to handle multiple elements
- Structuring logic into small, focused functions (`checkWinner`, `showWinner`, `resetGame`, etc.)
