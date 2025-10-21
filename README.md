# Snake Game

A classic Snake game implementation built with Python using the `curses` library for terminal-based gameplay.

## Features

- **Terminal-based gameplay** with smooth animations
- **Dynamic speed increase** as the snake grows longer
- **Score tracking** with real-time display
- **Collision detection** for walls and self-collision
- **Food generation** with collision avoidance
- **Keyboard controls** using arrow keys

## Requirements

- Python 3.x
- `curses` library (included in standard Python installation on Unix/Linux/macOS)
- For Windows users: Install `windows-curses` package

## Installation

1. Clone this repository:
```bash
git clone https://github.com/robertisaacs-hash/python_snake.git
cd python_snake
```

2. For Windows users, install the required dependency:
```bash
pip install windows-curses
```

## How to Play

1. Run the game:
```bash
python snake.py
```

2. **Controls:**
   - **Arrow Keys**: Move the snake (Up, Down, Left, Right)
   - **ESC**: Exit the game

3. **Objective:**
   - Guide the snake to eat food (marked with `#`)
   - Avoid hitting the walls or the snake's own body
   - Try to achieve the highest score possible!

## Game Mechanics

- The snake starts with 3 segments at position (4,4), (4,3), (4,2)
- Food appears randomly on the game board (marked with `#`)
- Each food consumed increases the score by 1 and grows the snake by 1 segment
- Game speed increases as the snake grows longer
- The game ends when the snake hits a wall or itself

## Technical Details

- **Window Size**: 60 columns × 20 rows
- **Game Speed**: Dynamic (150ms base, decreases as snake grows)
- **Snake Representation**: `*` character
- **Food Representation**: `#` character
- **Playable Area**: Inner window area (excluding borders)

## Code Structure

- `snake.py`: Main game file containing all game logic
  - Window setup and configuration
  - Game loop with input handling
  - Collision detection
  - Food generation and consumption
  - Score tracking and display

## Screenshots

The game runs in your terminal and looks like this:
```
┌──────────────────────────────────────────────────────────┐
│Score 5                                                   │
│                                                          │
│                                                          │
│    ***                                                   │
│                                                          │
│      #                                                   │
│                                                          │
│                                                          │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. Some ideas for improvements:

- Add pause functionality
- Implement high score persistence
- Add color support
- Create different difficulty levels
- Add sound effects

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Robert Isaacs** - [robertisaacs-hash](https://github.com/robertisaacs-hash)

---

Enjoy playing Snake! 🐍