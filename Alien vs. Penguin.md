# Maze Race to the Castle

This is an interactive browser-based game where two characters, an **alien (👽)** and a **penguin (🐧)**, race toward a **castle (🏰)** located randomly within a procedurally generated maze. The objective is to reach the castle first while avoiding each other and navigating the maze's complex structure.

## Features

1. **Procedurally Generated Maze**:
   - The maze is randomly generated each time the game is loaded.
   - Every maze is unique, providing endless replayability.

2. **Dynamic Characters**:
   - The **alien (👽)** and the **penguin (🐧)** start at opposite corners of the maze.
   - Both characters dynamically calculate the shortest path to the castle.

3. **Castle**:
   - A **castle (🏰)** is placed randomly within the maze.
   - The first character to reach the castle wins.

4. **Collision Handling**:
   - The alien and penguin avoid crossing paths, ensuring a fair race.

5. **Interactive Gameplay**:
   - Click on the canvas to start the game.
   - Watch as the alien and penguin race toward the castle.

## How It Works

- **Maze Generation**:
  - The maze is created using a randomized depth-first search algorithm.
  - Each cell in the maze has walls, which are removed to create paths.

- **Pathfinding**:
  - Both the alien and penguin calculate the shortest path to the castle using a Breadth-First Search (BFS) algorithm.

- **Randomization**:
  - The castle's location is randomized at the start of the game.
  - This ensures varied gameplay experiences.

## How to Play

1. Open the HTML file in any modern web browser.
2. The maze, characters, and castle will be generated automatically.
3. Click anywhere on the canvas to start the race.
4. Watch the alien and penguin navigate through the maze to reach the castle.
5. The game ends when either the alien or the penguin reaches the castle first, and a winner is declared.

## Code Overview

### Main Components

1. **Maze Generation**:
   - A `Cell` class represents each maze cell.
   - Walls are removed between neighboring cells to create paths.

2. **Character Movement**:
   - The alien and penguin independently calculate their paths to the castle.
   - Movement is animated step-by-step toward the target.

3. **Event Handling**:
   - A click event starts the race.

4. **Rendering**:
   - The maze and characters are rendered on a `canvas` element.

### Key Variables

- `alien`: Represents the alien's current position and emoji.
- `penguin`: Represents the penguin's current position and emoji.
- `castle`: Represents the castle's position and emoji.
- `maze`: A 2D array representing the maze structure.

## Customization

- **Adjust Speeds**:
  - Modify `alienSpeed` and `penguinSpeed` to change the movement speeds of the characters.

- **Maze Size**:
  - Adjust `cellSize` to make the maze cells larger or smaller.
  - The number of rows and columns in the maze automatically adjusts based on the canvas size and cell size.

## Future Enhancements

- Add power-ups for characters to temporarily boost speed.
- Implement obstacles within the maze for added difficulty.
- Introduce multiple levels with increasing complexity.

## Compatibility

This game is compatible with all modern browsers that support the HTML5 `<canvas>` element and JavaScript ES6.

## License

This project is open-source and licensed under the MIT License. Feel free to modify and distribute it as needed.
 