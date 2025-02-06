# Fireworks Trail Canvas Animation

## Description
This project is an interactive **HTML5 Canvas** animation that creates vibrant, glowing fireworks trails following the user's mouse movements. Each firework particle glows in random colors and fades away within **3 seconds**, creating a mesmerizing display. Additionally, a **real-time counter** in the top-right corner displays the number of visible particles currently on the canvas.

## Features
- **Dynamic Fireworks Effect:** Colorful particles explode along the mouse path with glowing effects.
- **Smooth Fading:** Particles fade out over time for a natural visual experience.
- **Real-Time Particle Counter:** Displays the current number of visible particles.
- **Performance Optimized:** Efficient rendering ensures smooth performance even with a large number of particles.

## Technologies Used
- **HTML5** for structure
- **CSS3** for basic styling
- **JavaScript** for canvas animation and interactivity

## How to Run
1. **Download or Clone** this repository.
2. Open the `index.html` file in any modern browser (**Google Chrome**, **Firefox**, etc.).
3. Move your mouse over the canvas to generate fireworks!

## Customization
- **Particle Lifespan:** Adjust the fade speed by modifying `particle.alpha -= 0.01` in the JavaScript code.
- **Particle Quantity:** Increase the number of particles per firework in the `createParticles()` function.
- **Colors and Glow:** Customize the glow intensity and color randomness in the `drawParticles()` function.

## License
This project is open-source and available for free use and modification.

## Acknowledgments
Inspired by creative canvas animations and interactive user experiences to add fun and visual appeal.
