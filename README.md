# 🧩 WordFall

![Version](https://img.shields.io/badge/version-1.0.0-cyan)
![License](https://img.shields.io/badge/license-MIT-purple)
![Style](https://img.shields.io/badge/style-Retro%20Cyberpunk-yellow)

**WordFall** is an arcade-style browser game that fuses the falling-block mechanics of Tetris with crossword puzzle logic. Set in a neon, retro-futuristic interface, players must manipulate falling tetrominos composed of letters to form words, clear the grid, and survive increasing speeds.

## 🎮 Game Overview

Blocks fall from the top of the screen in various shapes. Each block contains random letters (weighted between vowels and consonants). Your goal is to arrange these blocks to form valid English words (3 letters or more) horizontally or vertically.

When a word is formed:
1. The letters explode and clear from the grid.
2. Points are awarded based on word length.
3. Remaining blocks obey gravity and fall to fill empty spaces (potentially creating chain reactions!).

## ✨ Key Features

* **Hybrid Gameplay:** Classic block stacking meets anagram solving.
* **Physics System:** Blocks settle and fall when support is removed, allowing for strategic combos.
* **Dynamic Dictionary:** Validates against a comprehensive English dictionary (fetched dynamically).
* **Progressive Difficulty:** The game speeds up as you clear words and level up.
* **Retro Aesthetics:** 8-bit typography ("Press Start 2P"), neon glowing borders, and a dark mode interface.
* **Synthesized Audio:** Real-time sound effects generated via **Tone.js**.
* **Responsive:** Built with Tailwind CSS for layout adaptation.

## 🕹️ Controls

| Key | Action |
| :--- | :--- |
| **⬅️ Left Arrow** | Move Piece Left |
| **➡️ Right Arrow** | Move Piece Right |
| **⬇️ Down Arrow** | Soft Drop (Speed Up) |
| **Spacebar** | Rotate Piece |
| **P** | Pause / Resume Game |

## 🚀 How to Run

Since WordFall is built as a single-file application using CDNs, no build process or package manager (npm/yarn) is required.

### Prerequisites
* An active **Internet Connection** is required to load:
    * The Dictionary file (`words_alpha.txt`).
    * Tailwind CSS.
    * Tone.js (Audio).
    * Google Fonts.

### Steps
1.  Download the `index.html` file (containing the source code).
2.  Open the file directly in any modern web browser (Chrome, Firefox, Edge, Safari).
3.  Click **"Start Game"** to initialize the audio engine and begin.

## 🛠️ Technical Stack

* **Core:** HTML5, vanilla JavaScript (ES6+).
* **Rendering:** HTML5 `<canvas>` API for the game grid.
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN).
* **Audio:** [Tone.js](https://tonejs.github.io/) (via CDN) for procedural sound synthesis.
* **Data:** Fetches word list dynamically from `dwyl/english-words`.

## 📝 Rules & Scoring

1.  **Valid Words:** Must be **3 letters** or longer.
2.  **Direction:** Words can be formed Horizontally (Left-to-Right) or Vertically (Top-to-Bottom).
3.  **Game Over:** The game ends if the stack of blocks reaches the top of the grid.
4.  **Level Up:** Cleared words increase the level counter. Higher levels increase the drop speed of pieces.

## 🔮 Future Improvements

* [ ] Local High Score saving (using LocalStorage).
* [ ] "Hold Piece" functionality.
* [ ] Mobile touch controls.
* [ ] Particle effects on word clearing.

## 📄 Credits

* **Font:** "Press Start 2P" by CodeMan38 (Google Fonts).
* **Dictionary:** Sourced from [dwyl/english-words](https://github.com/dwyl/english-words).

---
*Enjoy the game!*
