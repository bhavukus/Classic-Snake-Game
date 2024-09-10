# Classic Snake Game

A classic and simple **Snake Game** implemented in Java using Swing and AWT libraries. The game allows the user to control the snake with arrow keys, grow by eating blue apples, and avoid collisions with the walls or its own body. The game incorporates real-time rendering and smooth gameplay mechanics, along with score tracking.

## Table of Contents
- [Project Overview](#project-overview)
- [Game Objective](#game-objective)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [How to Play](#how-to-play)
- [Setup and Installation](#setup-and-installation)
- [Code Structure](#code-structure)
  - [SnakeGame.java](#snakegamejava)
  - [GamePanel.java](#gamepaneljava)
  - [GameFrame.java](#gameframejava)
- [Key Concepts and Algorithms](#key-concepts-and-algorithms)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## Project Overview

This **Snake Game** project is a Java-based desktop application that recreates the classic Snake game. The game mechanics are simple: control a snake, eat food (blue apples), and avoid crashing into your own body or the game boundaries. With each apple eaten, the snake grows longer, making it more difficult to navigate. The game runs continuously until the snake collides with either its own body or the game walls.

The project demonstrates the application of object-oriented programming principles, real-time game development using the Java Swing framework, and basic data structures for handling the snake’s movement and collisions.
![Screenshot 2024-04-15 113907](https://github.com/user-attachments/assets/333ec8d2-446c-4d69-81a5-5a27accefca5)
![Screenshot 2024-04-15 113646](https://github.com/user-attachments/assets/b9dd9925-d731-4bb6-956d-5b0824f6eb84)


---

## Game Objective

The objective of the game is to control the snake and eat as many apples as possible to achieve a high score. Each apple eaten makes the snake grow longer, which increases the difficulty. The game ends when the snake collides with itself or the walls.

---

## Features

- **Real-time Snake Movement**: Smooth, responsive snake movement using keyboard arrow keys.
- **Apple Consumption & Growth**: The snake grows longer every time it eats an apple.
- **Score Tracking**: Displays the player's score based on the number of apples eaten.
- **Collision Detection**: Detects collisions between the snake and walls or its own body, ending the game if a collision occurs.
- **Game Over Screen**: Displays a "Game Over" message with the player's final score when the game ends.
- **Dynamic Gameplay**: The snake's increasing length adds a natural difficulty progression.

---

## Technologies Used

- **Java**: The core programming language used to implement the game logic.
- **Java Swing**: Used to create the game window, handle painting, and provide the graphical user interface (GUI).
- **AWT (Abstract Window Toolkit)**: Used for handling keyboard events and drawing components.
- **Object-Oriented Programming (OOP)**: The game is structured using OOP principles to manage game states, rendering, and user interaction.

---

## How to Play

- **Movement**: Control the snake's direction using the arrow keys (Up, Down, Left, Right).
- **Objective**: Eat the blue apples that appear on the screen to grow the snake.
- **Scoring**: Each apple eaten increases the snake's length and your score.
- **Avoid**: Don't crash into the walls or your own snake's body.
- **End of Game**: The game ends when the snake collides with itself or the game boundaries. A "Game Over" message along with your score is displayed.

---

## Setup and Installation

Follow these instructions to run the Snake Game on your local machine:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/bhavukus/Classic-Snake-Game.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd Classic-Snake-Game
    ```

3. **Compile the Java files**:
    ```bash
    javac *.java
    ```

4. **Run the game**:
    ```bash
    java ClassicSnakeGame
    ```

The game window will open, and you can start playing by using the arrow keys to control the snake.

---

## Code Structure

This project is divided into three main files:

### 1. **SnakeGame.java**
This is the main class that sets up the game window using the JFrame class. It also initializes the game by adding the game panel where the actual game logic is rendered.

Key responsibilities:
- Creating the game window (`JFrame`).
- Starting the game and setting up the game panel (`GamePanel`).

### 2. **GamePanel.java**
The heart of the game. This class handles the game logic, including snake movement, collision detection, rendering, and apple generation. It continuously listens for user input and updates the snake's state in real-time.

Key responsibilities:
- **Rendering**: Drawing the snake and the apples on the screen.
- **Movement**: Moving the snake based on user input (keyboard events).
- **Collision Detection**: Checking if the snake has collided with the walls or its own body.
- **Score Handling**: Keeping track of the player's score.
- **Game Loop**: Implemented using a `Timer` for continuous updates and rendering.

### 3. **GameFrame.java**
This class is responsible for managing the JFrame (game window) and initializing the game panel.

Key responsibilities:
- **Window Management**: Creating a window (`JFrame`) and adding the `GamePanel` to it.

---

## Key Concepts and Algorithms

### 1. **Snake Movement**
The snake's movement is achieved by shifting the position of each body part based on the direction of the head. The snake's direction is controlled by arrow keys.

### 2. **Collision Detection**
- **Self-collision**: The game checks if the head of the snake collides with any of its body parts.
- **Wall collision**: The game checks if the snake’s head touches the game window boundaries.

### 3. **Apple Consumption**
A random apple is placed on the game board. When the snake's head touches the apple, the snake grows by one unit, and the score is incremented.

---

## Future Improvements

While this project is fully functional, several improvements can be made:
- **Difficulty Levels**: Add levels of difficulty where the snake moves faster as the score increases.
- **Sound Effects**: Implement sound effects for apple consumption and collisions.
- **Multiple Themes**: Provide different color themes for the game board and snake.
- **Leaderboard**: Add a leaderboard to track high scores.

---

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code as long as you provide proper attribution. See the [LICENSE](LICENSE) file for details.
