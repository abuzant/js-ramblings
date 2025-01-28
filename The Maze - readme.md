# Maze Game: Alien and Penguin

## Overview
This project is a fun and interactive maze game implemented using HTML5 canvas and JavaScript. The game generates a random maze with exactly one correct path connecting:

- **An Alien (👽)** at one corner.
- **A Penguin (🐧)** at the opposite corner.

When the page loads, the maze is created. On clicking the canvas, the alien starts moving along the correct path to reach the penguin. The time taken for the alien to complete the journey is displayed at the end.

---

## Features

### Maze
- **Randomly Generated Maze**: Each page load creates a unique maze with one correct solution path.
- **Visual Representation**: The maze is drawn using grid cells, and walls separate paths.

### Alien and Penguin
- **Start and End Points**: The alien starts at the top-left corner, and the penguin is placed at the bottom-right corner.

### Animation
- **Interactive Movement**: The alien moves through the maze along the correct path upon the first click on the canvas.
- **Trail Effect**: A yellow trail is left behind as the alien moves, visually highlighting the path it takes.
- **Time Tracking**: The time taken for the alien to reach the penguin is displayed in milliseconds.

### Customization
- **Adjustable Alien Speed**: Control how fast the alien moves by modifying the `alienSpeed` variable in milliseconds.

---

## How It Works

### Maze Generation
The maze is generated using a depth-first search algorithm with backtracking. Walls are removed between cells to create paths, ensuring one valid path connects the alien and penguin.

### Pathfinding
The game uses a breadth-first search (BFS) algorithm to find the shortest path from the alien to the penguin.

### Animation
The alien moves step-by-step along the calculated path, leaving a trail behind. The speed of movement is controlled by the `alienSpeed` variable.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/maze-alien-penguin.git
   ```
2. Navigate to the project directory:
   ```bash
   cd maze-alien-penguin
   ```
3. Open `index.html` in any modern web browser.

---

## Usage

1. Open the `index.html` file in your browser.
2. Watch the randomly generated maze appear on the canvas.
3. Click anywhere on the canvas to start the alien’s journey to the penguin.
4. Observe the yellow trail as the alien moves, and see the total time taken once it reaches the penguin.

---

## Customization

### Alien Speed
You can adjust the alien’s movement speed by modifying the `alienSpeed` variable in the script:
```javascript
const alienSpeed = 50; // Speed in milliseconds between moves
```

### Maze Size
To change the maze dimensions, modify the `cols` and `rows` variables:
```javascript
const cols = 40; // Number of columns in the maze
const rows = 40; // Number of rows in the maze
```

### Trail Effect
The alien leaves a yellow trail. You can customize the trail's color or size in the `drawTrail` function:
```javascript
function drawTrail(x, y) {
    ctx.beginPath();
    ctx.arc(x * cellSize + cellSize / 2, y * cellSize + cellSize / 2, cellSize * 0.1, 0, Math.PI * 2);
    ctx.fillStyle = "yellow"; // Change trail color here
    ctx.fill();
}
```

---

## Contributing
Feel free to fork this project and submit pull requests with improvements, optimizations, or new features.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Preview
![Maze Game Preview](preview.gif)

---

Enjoy the game and have fun exploring the maze!
