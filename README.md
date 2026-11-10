# Rock Paper Scissors

A browser-based Rock Paper Scissors game built with HTML, CSS and vanilla JavaScript. Play against the computer, and the scoreboard keeps track of your wins and the computer's wins.

## Features

- Play against a computer opponent that picks randomly
- Click a rock, paper or scissors icon to make your move
- Live scoreboard for **You** and **Comp**
- Result message after every round, with colour feedback:
  - Green when you win
  - Red when you lose
  - Dark blue when the round is a draw
- Hover effect on the choice buttons

## Tech Stack

- HTML5
- CSS3 (Flexbox)
- JavaScript (ES6)

## How to Play

1. Click one of the three icons: **Rock**, **Paper** or **Scissors**.
2. The computer picks its move at random.
3. The winner is decided by the classic rules:
   - Rock beats Scissors
   - Scissors beats Paper
   - Paper beats Rock
4. The score updates after each round, and a message shows who won.
5. If both choose the same move, the round is a draw and nobody scores.

## Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/ssukhdeep02-git/rock-paper-scissors.git
   ```
2. Open the folder:
   ```bash
   cd rock-paper-scissors
   ```
3. Open `index.html` in your browser, or use the **Live Server** extension in VS Code.

No installation or build step is needed.

## Project Structure

```
rock-paper-scissors/
├── images/        # rock, paper and scissors icons
├── index.html     # Page structure
├── style.css      # Styling
├── app.js         # Game logic
└── README.md
```

## How It Works

- `genCompChoice()` picks a random move from `["rock", "paper", "scissors"]` using `Math.random()`.
- Each choice element has an `id` (`rock`, `paper`, `scissors`), which is read on click to get the player's move.
- `playGame()` compares the two moves. A matching pair calls `drawGame()`, otherwise it decides the winner and calls `showWinner()`.
- `showWinner()` updates the score, the message text and the message colour.

## Credits

Based on the Rock Paper Scissors project from the Apna College JavaScript series.

## Author

**Sukhdeep Singh Sidhu**
- GitHub: [ssukhdeep02-git](https://github.com/ssukhdeep02-git)
- LinkedIn: [Sukhdeep Sidhu](https://www.linkedin.com/in/sukhdeep-sidhu-60698b109/)
