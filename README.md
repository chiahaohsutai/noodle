# Noodles

A simple implementation of the classic Snake game built in Rust using the `macroquad` game framework.

This project was created as a hands-on introduction to Rust. Rather than learning the language exclusively through tutorials, I wanted to build a complete application that would expose me to Rust's ownership model, structs, enums, pattern matching, state management, and event-driven programming. Snake provided a straightforward but engaging project that touches many fundamental programming concepts while remaining small enough to complete as a beginner.

<img width="350" alt="Gameplay Screenshot" src="https://github.com/user-attachments/assets/2433b10a-d892-432b-a7ca-4fb01e4452ef">

## Why This Project?

Learning a new programming language is often easier when building something tangible. I chose Snake because it combines several common game development concepts:

- Real-time user input
- Game loops
- State management
- Collision detection
- Dynamic data structures
- Rendering graphics to the screen

The `macroquad` crate provided a lightweight way to build a graphical application without the complexity of a full game engine, allowing me to focus primarily on learning Rust and its ecosystem.

## Features

### Movement
- Control the snake using either **WASD** or the **Arrow Keys**.
- The snake moves continuously in the selected direction.
- Reverse movement is prevented to avoid immediate self-collisions.

### Food System
- Food spawns at random locations across the board.
- Consuming food increases the snake's length.
- A new piece of food is generated after each successful collection.

### Collision Detection
- The game ends when the snake collides with itself.
- This implementation does not include walls.
- Moving beyond the edge of the screen causes the snake to wrap around and reappear on the opposite side.

### Progressive Difficulty
- The snake's movement speed increases after eating food.
- Speed growth is capped to keep the game playable.

## Controls

| Key | Action |
|------|---------|
| `W`, `A`, `S`, `D` | Move Snake |
| Arrow Keys | Move Snake |
| `Enter` | Start Game |
| `Q` | Quit Game |
| `Esc` | Close Application |

## Installation

### Prerequisites

- Rust
- Cargo (included with Rust)

Install Rust from:

https://www.rust-lang.org/tools/install

### Running the Game

Clone the repository:

```bash
git clone <repository-url>
```

Navigate to the project directory:

```bash
cd rusty-snake
```

Build and run:

```bash
cargo run
```

Enjoy!
