
<!---
============================================================================
                  CURSOR AI INSTRUCTIONS - DO NOT MODIFY
============================================================================
-->

<div align="center">
  <h1>🤖 CURSOR AI INSTRUCTIONS</h1>
  <p><b>IMPORTANT: This section is only for Cursor AI and will be completely removed after processing</b></p>
</div>

---

## AI Task: Complete README Transformation

Hello Cursor AI! Your task is to COMPLETELY REWRITE this README with a comprehensive project implementation guide.

### Critical Requirements:

1. **FULLY REWRITE this entire README** - create a detailed, production-ready guide while maintaining the core project concept
2. **Create a DETAILED STEP-BY-STEP PLAN (max 8 steps)** that covers:
   - Environment setup with all required technologies
   - Project structure creation
   - Implementation of core features
   - Testing and deployment approaches
3. **Tailor content to the user's profile:**
   - User's Experience Level: `Beginner`
   - User's Available Time: `A Few Hours`
4. **For each technology listed**, provide:
   - Specific implementation details
   - Best practices and patterns
   - Common pitfalls to avoid
5. **Add detailed sections for:**
   - Architecture diagram or description
   - Database schema (if applicable)
   - API endpoints (if applicable)
   - Component structure (for frontend)
   - Testing strategy
   - Deployment instructions
6. **Provide code examples** for critical project parts
7. **REMOVE THESE INSTRUCTIONS COMPLETELY** after your rewrite

Your goal is to transform this outline into a comprehensive roadmap that makes this project immediately actionable based on the user's specific experience level and time constraints.

### ⚠️ CRITICAL FIRST STEP ⚠️

**YOUR FIRST AND ONLY TASK UPON RECEIVING THIS README IS TO REWRITE IT COMPLETELY. DO NOT START IMPLEMENTING THE PROJECT OR WRITING ANY CODE YET.**

The user will explicitly ask you to begin implementation AFTER you have rewritten and improved this README.

<!---
============================================================================
                 END OF CURSOR AI INSTRUCTIONS
============================================================================
-->


# REWIND RAIDERS 3D - Initial Prototype

## Project Overview
Create an initial prototype for a 3D pixelated first-person shooter web game using Three.js and JavaScript. The gameplay core will focus on enemy AI, with a functional rewind mechanic and basic game controls.


> **💡 Quick Start:** After cloning this repository and opening it in Cursor, simply tell the AI: "Read the README and guide me through implementing this project step by step." Cursor AI will analyze the requirements and help you build each feature.


## User Profile
- **Experience Level:** Beginner
- **Available Time to Complete:** A Few Hours

## Technologies
- **HTML5**: Used for structuring and presenting content on the web.
- **Three.js**: Used for creating and rendering 3D graphics in the browser.
- **JavaScript**: Used for creating game logic, handling user input, and updating the game state.
- **dat.GUI**: Used for debugging and visualizing game parameters.
- **localStorage**: Used for saving and loading game settings and scores.
- **GLSL**: Used for creating custom shaders for visual effects, such as glitches.


## Development Steps
### 1. Set up the project structure
Create a new HTML file, initialize Three.js, and set up a basic scene with a camera and a renderer.

### 2. Implement basic game controls
Add keyboard and mouse event listeners to handle player movement and shooting.

### 3. Create a basic enemy AI
Implement a simple enemy AI using JavaScript, with enemies that can move and attack the player.

### 4. Implement the rewind mechanic
Create a functional rewind mechanic that allows the player to rewind time and create clones.

### 5. Add basic graphics and visual effects
Add pixelated textures, simple lighting, and a glitch shader to enhance the game's visual style.

### 6. Test and refine the game
Test the game, fix bugs, and refine the gameplay experience to achieve a smooth 60 FPS.

### 7. Add a simple level and UI
Create a basic level with platforms and enemies, and add a simple user interface to display score and settings.


## Main Features
Features will be added soon



## Getting Started
Instructions will be added soon

## Resources
- [Three.js Documentation](https://threejs.org/docs/) (documentation)
- [dat.GUI Tutorial](https://codepen.io/tmrdevelops/pen/MwvrJv) (tutorial)
- [GLSL Shader Tutorial](https://thebookofshaders.com/) (tutorial)
- [JavaScript and HTML5 Game Development](https://www.packtpub.com/product/html5-game-development-by-example/9781849691741) (book)
- [Game Development with Three.js](https://www.udemy.com/course/threejs/) (course)


## AI Coding Prompts

Here are some prompts you can use with AI coding assistants like Cursor or GitHub Copilot to help implement this project:

### Prompt 1
```
Create a new JavaScript file and set up the basic structure for the game. Use HTML5 to create an index.html file and include the Three.js library. Initialize the scene and camera, and add a basic game loop using JavaScript. Copy and paste the following code as a starting point:

<script>
  // Initialize Three.js scene and camera
  const scene = new THREE.Scene();
  const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
  
  // Add lights and renderer
  const light = new THREE.DirectionalLight(0xffffff, 1);
  scene.add(light);
  const renderer = new THREE.WebGLRenderer({canvas: document.getElementById('canvas'), antialias: true});
  renderer.setSize(window.innerWidth, window.innerHeight);
  
  // Render the scene
  function animate() {
    requestAnimationFrame(animate);
    renderer.render(scene, camera);
  }
  animate();
</script>
```

### Prompt 2
```
Implement the core gameplay mechanics, including enemy AI and the rewind mechanic. Use JavaScript to create enemy objects and assign them movement patterns and behaviors. Add a rewind function that allows the player to rewind time and replay the game. Use the dat.GUI library to create a GUI interface for debugging and visualizing game parameters. Copy and paste the following code as a starting point:

// Create an enemy class
class Enemy {
  constructor(x, y, z) {
    this.position = new THREE.Vector3(x, y, z);
    this.velocity = new THREE.Vector3(0, 0, 0);
  }
  update() {
    // Update enemy movement
  }
}

// Create a game state class
class GameState {
  constructor() {
    this.time = 0;
    this rewindEnabled = true;
  }
  update() {
    // Update game state
  }
}

// Create the game loop
function update() {
  // Update enemies
  enemies.forEach((enemy) => enemy.update());
  // Update game state
  gameState.update();
}

// Implement the rewind mechanic
function rewind() {
  // Rewind game state and replay the game
}
```

### Prompt 3
```
Add advanced features to the game, such as custom shaders for visual effects and local storage for saving and loading game settings and scores. Use GLSL to create custom shaders and add them to the game scene. Implement local storage using the localStorage API. Copy and paste the following code as a starting point:

// Create a custom shader
const shaderMaterial = new THREE.ShaderMaterial({
  vertexShader: "#version 300 es\nuniform vec3 color;\nvoid main() {\n  gl_Position = vec4(position, 1.0);\n  gl_FragColor = vec4(color, 1.0);\n}",
  fragmentShader: "#version 300 es\nuniform vec3 color;\nvoid main() {\n  gl_FragColor = vec4(color, 1.0);\n}",
  uniforms: {color: {value: new THREE.Color(0xff0000)}}
});

// Add the shader material to the scene
const shaderMesh = new THREE.Mesh(geometry, shaderMaterial);
scene.add(shaderMesh);

// Implement local storage for saving and loading game settings and scores
function saveGame() {
  // Save game state to local storage
}
function loadGame() {
  // Load game state from local storage
}
```


Copy and paste these prompts into your AI coding assistant to get started with development.


---
*Generated by [CodeSpark](https://github.com/YOUR_USERNAME/codespark)*
