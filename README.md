# 🎯 Angle Predictor

A fun and interactive browser-based game where players estimate a randomly generated angle between **0° and 360°**. The game provides directional **Hot/Cold** hints, a **5-life system**, and a **history log** to help players narrow down the correct answer.

---

## Features

- Random angle generation (0°–360°)
- Visual angle diagram using SVG
- Five-life (heart) system
- Hot/Cold feedback based on guess accuracy
- Directional hints (Too High / Too Low)
- Guess history log
- Green success message when correct
- Red feedback for incorrect guesses
- Automatic Game Over after all lives are lost
- Single button that changes from **Guess** to **New Game**
- Responsive design for desktop and mobile devices

---

## How to Play

1. Observe the displayed angle.
2. Enter your guess (between **0° and 360°**).
3. Click **Guess**.
4. Read the feedback:
   - 🎯 Perfect Match
   - 🔥 Very Hot
   - 🌞 Hot
   - 🥶 Cold
   - 🧊 Freezing
5. Continue until:
   - You guess the exact angle, or
   - You run out of all five lives.
6. Press **New Game** to play again.

---

## Feedback Guide

| Feedback | Meaning |
|----------|---------|
| 🎯 PERFECT MATCH | Correct angle |
| 🔥 VERY HOT | Within 5° of the target |
| 🌞 HOT | Guess is close but too high |
| 🥶 COLD | Guess is close but too low |
| 🧊 FREEZING | More than 60° away |

---

## Lives System

The player starts with:

❤️❤️❤️❤️❤️

Each incorrect guess removes one heart.

Example:

```
❤️❤️❤️🖤🖤
```

After five incorrect guesses, the game ends and reveals the correct angle.

---

## Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- SVG Graphics

No external libraries or frameworks are required.

---

## Project Structure

```
AnglePredictor/
│
├── index.html
└── README.md
```

---

## Game Logic

- A random target angle is generated.
- The target line and angle arc are drawn using SVG.
- Every guess calculates the shortest angular distance.
- Feedback is generated based on:
  - Distance from target
  - Whether the guess is above or below the correct angle.
- The game tracks:
  - Remaining lives
  - Guess history
  - Game state

---

## Responsive Design

The interface automatically adapts to smaller screens by:

- Stacking panels vertically
- Reducing SVG size
- Maintaining scrollable history
- Preserving gameplay on mobile devices

---

## Learning Objectives

This project demonstrates:

- DOM manipulation
- SVG graphics
- Event handling
- Conditional logic
- Random number generation
- Responsive web design
- State management in JavaScript

---

## Future Improvements

Possible enhancements include:

- Difficulty levels
- Timer mode
- Scoreboard
- Best score tracking
- Sound effects
- Multiplayer mode
- Keyboard shortcuts
- Animated feedback
- Statistics dashboard
- Dark/Light theme switch

---

## Browser Compatibility

Compatible with modern browsers including:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari
- Opera

---

## Author

Created as a JavaScript practice project for learning interactive game development, SVG graphics, and user interface design.

---

## License

This project is open-source and may be modified, distributed, and used for educational or personal purposes.
