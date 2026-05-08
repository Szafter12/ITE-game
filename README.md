# Feline Slayer
A Pixel Art Top-Down Wave Survival Shooter.

### What the project is
Feline Slayer is a classic-style 2D survival game where the player faces increasingly difficult waves of enemies. Built with **C++17** and **SFML 3.0**, the game features a top-down perspective, multiple enemy types, and a retro pixel-art aesthetic.

### Aim
This project was developed for the "Introduction to Computer Science" university course. The primary aim was to master **Object-Oriented Programming (OOP)** in C++ and game development fundamentals, such as managing the game loop, implementing collision detection, and handling resource management (textures, sounds, and animations) using the SFML library.

### Key Features
* **Wave-Based Combat:** Survival mechanics with increasing difficulty and varied enemy types (basic and fast).
* **Power-up System:** Temporary upgrades to enhance player performance during combat.
* **State Management:** Functional "Save/Load" system, death screens, and restart options.
* **Visual Effects:** Basic particle systems, hit feedback, and sprite animations for a polished feel.
* **Modern Workflow:** Project managed via **CMake** with a **FetchContent** approach for seamless dependency handling.

### Controls
* **Move:** `W` `A` `S` `D`
* **Aim:** `Mouse Cursor`
* **Shoot:** `Space`
* **Menu:** `Esc`
* **Quit Game:** `P`

### Challenges
* **Team Collaboration:** Coordinating work between multiple developers and merging different features.
    * **Solution:** Implemented a git-flow strategy where each team member worked on a dedicated branch, with weekly merge sessions and code reviews to resolve conflicts.
* **Resource Management:** Loading and disposing of assets efficiently without causing memory leaks or stuttering.
    * **Solution:** Developed a central Resource Manager to handle textures and sounds, ensuring each asset is loaded only once and remains accessible throughout the game life cycle.

### Setup or usage instructions

1. **Clone & Build:**
```bash
git clone [https://github.com/Szafter12/PI-game](https://github.com/Szafter12/PI-game)
cd PI-game
cmake -S . -B build
cmake --build build --config Debug
```
2. **Asset Deployment (Windows example)**
```bash
cp assets .\build\assets -Recurse
cd .\build\bin\Debug
```
3. **Run Application**
```bash
.\Game_PI.exe
```
Note: Visual Studio users can simply "Open Folder" as a CMake project and run via F5.

### Technical concepts used

- C++17 OOP: Inheritance and polymorphism for enemy and projectile logic.
- SFML 3.0: Handling graphics rendering, window management, and audio.
- JSON Integration: Using nlohmann/json for saving configurations and high scores.
- Game Physics: Simple AI pathfinding and AABB collision detection.
- CMake: Modern build system management and dependency fetching.

### Images/video demos

![Game screenshot](ss1.png)
