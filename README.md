# Asteroids Game 🚀

A classic arcade-style Asteroids game built with Python and Pygame. Destroy asteroids while avoiding collisions, and watch the difficulty increase as asteroids split into smaller pieces.

## Features

- **Classic Gameplay**: Rotate, thrust, and shoot to destroy asteroids
- **Progressive Difficulty**: Asteroids split into smaller pieces when destroyed
- **Event Logging**: Tracks game events and state for analysis
- **Smooth Physics**: Velocity-based movement system with proper collision detection

## Requirements

- Python 3.13+
- Pygame 2.6.1

## Installation

1. Clone the repository:
```bash
git clone https://github.com/arulzkash/Asteroids.git
cd Asteroids
```

2. Install dependencies using UV:
```bash
uv sync
```

Or with pip:
```bash
pip install pygame==2.6.1
```

## How to Play

Run the game:
```bash
uv run main.py
```

### Controls
- **A D**: Rotate your ship
- **W**: Thrust forward
- **S**: Thrust backward
- **Spacebar**: Shoot
- **ESC/Close Window**: Exit game

### Objective
- Destroy all asteroids on the screen
- Each destroyed asteroid may split into smaller ones
- Avoid colliding with asteroids!
- Game ends when you collide with an asteroid

## Project Structure

```
.
├── main.py              # Main game loop and event handler
├── player.py            # Player ship class
├── asteroid.py          # Asteroid class with splitting logic
├── shot.py              # Projectile/bullet class
├── asteroidfield.py     # Asteroid spawner and manager
├── circleshape.py       # Base class for circular objects
├── constants.py         # Game configuration values
├── logger.py            # Event and state logging system
├── pyproject.toml       # Project dependencies
└── README.md            # This file
```

## Game Configuration

Edit `constants.py` to customize game behavior:
- `SCREEN_WIDTH` / `SCREEN_HEIGHT`: Window size
- `PLAYER_SPEED`: Movement speed
- `PLAYER_SHOOT_SPEED`: Bullet speed
- `ASTEROID_SPAWN_RATE_SECONDS`: How often asteroids appear
- `ASTEROID_MAX_RADIUS`: Size of largest asteroids

## Logging

The game logs events to:
- `game_events.jsonl`: Individual events (asteroid_split, player_hit, etc.)
- `game_state.jsonl`: Game state snapshots during runtime

Useful for game analysis and debugging!

## Future Improvements

- [ ] Score system and high score tracking
- [ ] Sound effects and music
- [ ] Multiple lives/lives system
- [ ] Power-ups (shields, rapid fire, etc.)
- [ ] Menu and pause functionality
- [ ] Difficulty levels

## License

MIT License - feel free to use and modify!

## Author

Created as a Python learning project

---

**Enjoy playing!** 🎮
