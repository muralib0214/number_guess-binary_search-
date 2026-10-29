# NEXUS — Holographic Number Guessing Game

A binary-search guessing game with a premium sci-fi HUD and animated holographic core. The computer guesses a number you are thinking of; you tell it whether the guess is too high, too low, or correct.

## ✨ Browser experience

- **Premium sci-fi HUD:** layered translucent panels, technical telemetry, restrained cyan/blue lighting, and a dark atmospheric grid.
- **CSS 3D hologram:** floating glass number frame, illuminated core, rotating orbital rings, scan lines, and a projected floor.
- **Context-aware effects:** amber pulses for “too high,” cyan-blue pulses for “too low,” a mint-green particle celebration for a correct guess, and a red glitch warning if answers conflict.
- **Live telemetry:** possible numbers remaining, search reduction, current range, maximum expected guesses, and signal history.
- **Range controls:** custom integer ranges plus presets for 1–10, 1–100, 1–1,000, and −50–50.
- **Keyboard controls:** Left Arrow = too high, Right Arrow = too low, Enter = correct.
- **Responsive layout:** desktop three-column HUD, tablet adaptation, and mobile stacked layout.
- **Accessibility and resilience:** semantic controls, live status messages, visible keyboard focus, input validation, and reduced-motion support.

The browser version uses plain HTML, CSS, and JavaScript with a canvas particle effect. It does not require Three.js, a build step, package installation, a server, or external assets. The holographic depth is created with CSS 3D transforms and layered lighting, keeping it lightweight and compatible with GitHub Pages.

## 🚀 Run without cloning

Open the deployed GitHub Pages site in your browser (after Pages is enabled for the repository):

https://muralib0214.github.io/number_guess-binary_search-/

Or open `index.html` directly in any modern browser. No build command is needed.

## 🐍 Run the original Python game

Requires Python 3.x.

```bash
python number_guess.py
```

The original terminal game is preserved alongside the browser UI.

## 🧠 How binary search works

1. Inspect the midpoint of the current candidate range.
2. If the guess is too high, discard the upper part; if too low, discard the lower part.
3. Repeat until the target is found.

Each answer reduces the candidate set by about half. Time complexity is **O(log n)**.

| Candidate range size | Maximum guesses (approx.) |
| ---: | ---: |
| 100 | 7 |
| 1,000 | 10 |
| 1,000,000 | 20 |

## 📂 Project structure

```text
number_guess-binary_search-/
├── index.html       # Holographic browser UI and game logic
├── number_guess.py  # Original Python terminal game
└── README.md        # Project documentation
```

## 🛠️ Stack

- HTML5
- CSS3 (3D transforms, animation, responsive layout)
- Vanilla JavaScript
- Canvas 2D particles
- Python 3 (original terminal version)

## ♿ Motion preferences

Animations respect the operating system's `prefers-reduced-motion` preference. The core game logic and buttons remain usable without motion effects.

## 🔮 Possible next steps

- Optional sound design and user-controlled intensity
- Persisted personal best and game statistics
- Additional visual themes and challenge modes

## 👨‍💻 Author

Murali
