# Rotating Triangle with Bouncing Ball

## Overview
This project demonstrates an interactive HTML5 canvas animation featuring:

1. A rotating triangle that changes its rotation direction when clicked.
2. A bouncing ball constrained within the triangle's edges, dynamically increasing and decreasing its speed upon collision.

The animation is created using pure HTML5, CSS, and JavaScript, showcasing dynamic geometry, collision detection, and interactive features.

---

## Features

### Triangle
- **Rotating Triangle**: The triangle rotates continuously in the canvas.
- **Direction Toggle**: Clicking anywhere on the canvas reverses the direction of the triangle's rotation.

### Ball
- **Bouncing Ball**: A red ball bounces within the triangle, reflecting off the edges.
- **Dynamic Speed Adjustment**: The ball's speed alternates between increasing and decreasing upon each collision with an edge.

### Interaction
- **Mouse Click**: Toggle the triangle's rotation direction with a simple click.

---

## How It Works

### Collision Detection
The script calculates the ball's position relative to the triangle's edges using:
- **Point-to-Line Distance**: Determines if the ball touches an edge.
- **Reflection Logic**: Reflects the ball's velocity vector when a collision is detected.

### Dynamic Speed Adjustment
- When the ball collides with an edge, its speed alternates between increasing by 20% and decreasing by 20%.

### Triangle Rotation
- The triangle rotates continuously, with its rotation angle updated on each animation frame.
- The rotation direction toggles when the user clicks on the canvas.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/rotating-triangle-bouncing-ball.git
   ```
2. Navigate to the project folder:
   ```bash
   cd rotating-triangle-bouncing-ball
   ```
3. Open `index.html` in any modern web browser.

---

## Files

- `index.html`: The main file containing the animation code.
- `README.md`: Project documentation.

---

## Usage

1. Open the `index.html` file in your web browser.
2. Watch the triangle rotate and the ball bounce inside it.
3. Click anywhere on the canvas to toggle the triangle's rotation direction.

---

## Customization

You can customize the following parameters within the script:

1. **Triangle Size**: Adjust the `triangleSize` variable to change the size of the triangle.
2. **Ball Speed**: Modify the initial `dx` and `dy` values of the `ball` object to set its default speed.
3. **Rotation Speed**: Adjust the `rotateDirection` variable for faster or slower rotation.

---

## Contributing
Feel free to fork this project and submit pull requests for improvements or additional features.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Preview
![Preview of Rotating Triangle with Bouncing Ball](preview.gif)

---

Enjoy the animation and feel free to share your feedback!
 