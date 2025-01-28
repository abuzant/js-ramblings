# Underwater Fish and Prawn Simulation

## Overview
This project is an engaging underwater simulation implemented using HTML5 Canvas and JavaScript. The simulation creates a dynamic aquatic environment where:

- **Fish** move randomly, grow by eating smaller fish, and compete for survival.
- **Prawns** crawl horizontally along the bottom of the aquarium.
- **Bubbles** float from the bottom to the top, adding realism to the underwater scene.

The goal of the simulation is to create a visually appealing and interactive ecosystem where fish and prawns coexist, while bubbles add a sense of liveliness to the environment.

---

## Features

### 1. **Dynamic Fish Behavior**
- Each fish is represented by an emoji selected randomly from a predefined list.
- Fish vary in size, speed, and movement direction.
- Fish move freely across the canvas, bouncing off walls when they reach the boundaries.
- Collision Detection:
  - Larger fish consume smaller fish upon collision, growing in size.
  - The simulation ends when only one fish remains.

### 2. **Prawns Crawling on the Bottom**
- Prawns (`🦐`) crawl horizontally along the bottom of the aquarium.
- There are 32 prawns with sizes ranging from small to large.
- Prawns move back and forth, bouncing off the edges of the canvas.

### 3. **Bubbles Floating Upward**
- Air bubbles (`🫧`) rise from the bottom of the canvas to the top.
- A maximum of 24 bubbles are present at any given time.
- Bubbles vary in size and speed, disappearing when they leave the canvas.

### 4. **Interactive Environment**
- The simulation is fully dynamic, with all entities moving and interacting autonomously.
- The user is alerted when only one fish remains, marking the end of the simulation.

---

## Logic and Implementation

### 1. **Fish Class**
- Properties:
  - `x`, `y`: Position on the canvas.
  - `size`: Size of the fish, which increases when it consumes another fish.
  - `speed`: Movement speed.
  - `direction`: Current movement direction in radians.
  - `emoji`: Fish emoji representing the fish.
- Methods:
  - `draw()`: Updates the fish's position on the canvas.
  - `update()`: Adjusts the position and handles wall collisions.
  - `checkCollision(otherFish)`: Detects collisions with other fish and determines if a fish is eaten.

### 2. **Prawn Class**
- Properties:
  - `x`, `y`: Position, with `y` fixed at the bottom of the canvas.
  - `size`: Size of the prawn.
  - `speed`: Horizontal movement speed.
  - `emoji`: Always set to `🦐`.
- Methods:
  - `draw()`: Updates the prawn's position on the canvas.
  - `update()`: Handles horizontal movement and bouncing off the edges.

### 3. **Bubble Class**
- Properties:
  - `x`, `y`: Position on the canvas.
  - `size`: Size of the bubble.
  - `speed`: Vertical speed.
  - `emoji`: Always set to `🫧`.
- Methods:
  - `draw()`: Updates the bubble's position on the canvas.
  - `update()`: Moves the bubble upward and removes it when it leaves the canvas.

### 4. **Initialization Functions**
- `initializeFish()`: Creates and initializes the fish array.
- `initializePrawns()`: Creates and initializes the prawn array at the bottom of the canvas.
- `initializeBubbles()`: Adds bubbles to the bubble array if fewer than the maximum are present.

### 5. **Animation Loop**
- Continuously updates the position and behavior of all entities.
- Handles collisions between fish.
- Removes bubbles that leave the canvas.
- Ends the simulation when only one fish remains, displaying an alert with the final fish's size.

---

## How to Run
1. Copy the provided HTML code into an `.html` file.
2. Open the file in any modern web browser.
3. Enjoy the interactive underwater simulation!

---

## Customization Options
- **Fish and Prawn Counts**: Modify `numFish` and `numPrawns` variables to change the number of fish and prawns in the simulation.
- **Bubble Behavior**: Adjust `maxBubbles` to limit the number of bubbles and their sizes.
- **Emoji Selection**: Add or remove emojis from the `fishEmojis` array to customize fish appearances.
- **Speed and Sizes**: Tweak speed and size calculations for fish, prawns, and bubbles to create different dynamics.

---

## Future Enhancements
- **Predator-Prey Dynamics**: Introduce specific predator fish that target only certain types of fish.
- **User Interaction**: Allow users to add bubbles or fish with mouse clicks.
- **Scoring System**: Track the number of fish consumed and display a leaderboard.
- **Sound Effects**: Add ambient underwater sounds and effects for fish collisions.

---

Enjoy exploring the underwater world! 🌊🐟🦐🫧