# Crysknife Game Project

### 👾 Group Name: **Crysknife**

---

## 🎯 Project Goal

We are **Crysknife**, a team of developers passionate about creating immersive and engaging experiences through code.  
Our mission is to **build a complete game in Java**, focusing on strong gameplay mechanics, clean architecture, and polished design.

---

## 🧩 Overview

This repository contains the source code, assets, and documentation for our Java-based game project.  
The game is being developed using **object-oriented programming principles** and designed for **cross-platform compatibility**.

Key focuses include:
- 🕹️ Core gameplay loop and mechanics  
- 🎨 Visual and sound design integration  
- 🧠 Modular and maintainable codebase  
- 🧪 Continuous testing and iteration  

---

## 🛠️ Technologies & Tools

- **Language:** Java  
- **IDE:** IntelliJ IDEA  
- **Libraries:** SimpleGFX 
- **Version Control:** Git & GitHub  
- **Build Tool:** Maven?
---

## 📂 Repository Structure
Crysknife-Game/
Crysknife-Game/
│
├── 📁 src/
│ ├── 📁 main/
│ │ ├── 📁 game/
│ │ │ ├── Game.java # Main entry point (contains main loop)
│ │ │ ├── GameEngine.java # Core logic, updates, and rendering
│ │ │ └── GameLauncher.java # Initializes the game window and starts the engine
│ │ │
│ │ ├── 📁 entities/
│ │ │ ├── Entity.java # Base class for all entities (players, enemies, items)
│ │ │ ├── Player.java # Player entity
│ │ │ ├── Enemy.java # Enemy entity
│ │ │ └── NPC.java # Non-playable character logic
│ │ │
│ │ ├── 📁 graphics/
│ │ │ ├── Renderer.java # Handles drawing and rendering objects
│ │ │ ├── Sprite.java # Manages images/sprites
│ │ │ └── Animation.java # Handles animations
│ │ │
│ │ ├── 📁 input/
│ │ │ ├── InputHandler.java # Keyboard/mouse event processing
│ │ │ └── Controller.java # Optional gamepad support
│ │ │
│ │ ├── 📁 world/
│ │ │ ├── World.java # Manages maps, tiles, and entities
│ │ │ ├── Tile.java # Base class for map tiles
│ │ │ └── LevelLoader.java # Loads levels/maps from files
│ │ │
│ │ ├── 📁 ui/
│ │ │ ├── HUD.java # Heads-Up Display elements
│ │ │ ├── Menu.java # Main menu UI
│ │ │ └── Button.java # Generic UI button
│ │ │
│ │ ├── 📁 audio/
│ │ │ ├── Sound.java # Sound effect manager
│ │ │ └── Music.java # Background music controller
│ │ │
│ │ ├── 📁 utils/
│ │ │ ├── Constants.java # Game-wide constants
│ │ │ └── ResourceLoader.java # Loads assets (images, sounds, etc.)
│ │ │
│ │ └── 📁 physics/
│ │ ├── Collision.java # Collision detection
│ │ └── Movement.java # Handles movement and velocity
│ │
│ └── 📁 test/
│ └── GameTests.java # Unit tests
│
├── 📁 assets/
│ ├── 📁 images/ # Sprites, textures, UI icons
│ ├── 📁 sounds/ # Sound effects and music
│ └── 📁 levels/ # Map or level data
│
├── 📁 docs/
│ ├── design-doc.md # Design overview
│ └── roadmap.md # Development milestones
│
├── 📁 lib/ # External libraries (if any)
│
├── .gitignore
├── build.gradle or pom.xml # Build configuration
└── README.md # Project documentation
