# 🎯 Mindguess — Number Guessing Game

A beginner-friendly number guessing project powered by **binary search**. The computer can guess the number you're thinking of through the original Python terminal game, or you can play with the new polished, responsive browser interface.

## ✨ Browser UI

The web version includes:
- 🌙 Classy dark interface with lime and violet accents
- 📱 Responsive layout for desktop, tablet, and mobile
- 🎮 Interactive **Too high**, **Too low**, and **That's it!** controls
- 🎚️ Custom ranges and one-click presets (1–10, 1–100, 1–1,000, and −50–50)
- 📊 Search progress, numbers remaining, guess count, and guess history
- ⌨️ Keyboard shortcuts: **←** = too high, **→** = too low, **Enter** = correct
- ♿ Focus-visible controls, accessible live feedback, and reduced-motion support
- 🚫 Input validation and clear recovery when answers conflict

The browser game is implemented in plain HTML, CSS, and JavaScript. No frameworks, package installation, server, or external libraries are required.

## 🚀 Run the browser game

1. Download or clone this repository.
2. Open `index.html` in any modern browser.
3. Think of a number in the selected range and respond to the computer's guesses.

You can also use VS Code's Live Server extension if you prefer a local development server.

## 🐍 Run the original Python game

Requires Python 3.x and no external libraries.

```bash
git clone https://github.com/muralib0214/number_guess-binary_search-.git
cd number_guess-binary_search-
python number_guess.py
```

The terminal version asks you to choose a start and end range, then answers whether each computer guess matches your number and whether your number is higher or lower.

## 🧠 How binary search works

1. Find the middle of the current range.
2. Ask whether the target number is the guess, higher, or lower.
3. Discard the half that cannot contain the target.
4. Repeat until the number is found.

Each answer cuts the search range roughly in half, so the algorithm runs in **O(log n)** time.

| Range size | Maximum guesses (approximately) |
| ---: | ---: |
| 100 | 7 |
| 1,000 | 10 |
| 1,000,000 | 20 |

## 📂 Project structure

```text
number_guess-binary_search-/
├── index.html       # Interactive browser UI (HTML, CSS, JavaScript)
├── number_guess.py  # Original Python terminal game
└── README.md        # Project documentation
```

## 🛠️ Tech stack

- **Python 3** — original command-line implementation
- **HTML5, CSS3, JavaScript** — browser UI
- **Binary search** — core search strategy

## 🔮 Possible next steps

- Add sound and optional visual effects
- Save personal bests and play statistics locally
- Add more game modes and accessibility preferences

## 👨‍💻 Author

Murali — learning data structures, algorithms, and Python.

Contributions and suggestions are welcome.
