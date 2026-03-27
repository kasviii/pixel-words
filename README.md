# 🟩 PIXEL WORDS

> A retro pixel-style word game site with three classic game modes — playable solo or with a friend.

**Live demo:** [https://kasviii.github.io/pixel-words](https://kasviii.github.io/pixel-words)

---

## 🎮 Game Modes

### Wordle
Guess the hidden 5-letter word in 6 tries. After each guess, tiles reveal clues:
- 🟩 **Green** — correct letter, correct position
- 🟨 **Yellow** — correct letter, wrong position
- ⬛ **Grey** — letter not in the word

In solo mode, a new word is generated daily using a date seed (same word all day, changes at midnight). In 2-player mode, Player 1 sets the word.

### Hangman
Guess the hidden word one letter at a time before the figure is complete. You have **7 lives**. Each wrong guess draws another part of the hangman. In 2-player mode, Player 1 types any word for Player 2 to solve.

### Scramble
Unscramble the jumbled word before the timer runs out. Features:
- Difficulty-based timers (Easy: 40s, Medium: 30s, Hard: 20s)
- Hint system (costs 5 points)
- Skip option
- Score and streak tracking
- In 2-player mode, Player 1 sets up to 5 words for Player 2 to unscramble in sequence

---

## 👥 2-Player Mode

Each game mode supports a pass-and-play 2-player option:

1. Select a game mode
2. Choose **2 Players**
3. Player 1 types the secret word (hidden behind a password field)
4. A handoff screen prompts P1 to pass the device
5. Player 2 plays without ever seeing the word

---

## 🎯 Difficulty Levels

Available in solo Hangman and Scramble:

| Level | Word Complexity | Scramble Timer | Bonus Points |
|-------|----------------|----------------|--------------|
| Easy | Common 5-letter words | 40s | — |
| Medium | Moderate vocabulary | 30s | +5 pts |
| Hard | Challenging vocabulary | 20s | +10 pts |

---

## 📊 Stats

Your wins, current streak, and best streak are saved in `localStorage` and persist across sessions. Stats are tracked globally across all three game modes.

---

## 🛠️ Tech Stack

- Pure **HTML / CSS / JavaScript** — no frameworks, no dependencies
- **Google Fonts** — Press Start 2P (pixel font) + VT323 (retro terminal font)
- **Canvas API** — for the Hangman drawing and win confetti
- **localStorage** — for persistent stats across sessions

---

## 📁 Project Structure

```
pixel-words/
└── index.html    # entire game — one file
└── README.md
```

---

## ✨ Features

- Retro CRT scanline effect
- Pixel confetti on every win
- On-screen keyboard for Wordle
- Password-protected word entry for 2-player mode
- Seeded daily word for Wordle (same word all day)
- 400+ word bank shuffled randomly each session
- Fully responsive — works on mobile and desktop

---


*Built with 💚 and way too many pixels.*
