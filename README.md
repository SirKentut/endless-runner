# Endless Runner Game

This is an **endless runner** game utilizing **OpenGL** and **Unreal Engine**, primarily written in **C++**. The player controls a character that runs horizontally across the screen while avoiding obstacles. Inspired by classic endless runner games like **Run** and **Temple Run**, the game aims to provide an immersive and fast-paced experience.

## Table of Contents
- [Game Overview](#game-overview)
- [Tech Stack](#tech-stack)
- [Setup](#setup)
- [Project Structure](#project-structure)
- [How to Contribute](#how-to-contribute)
- [Important Notes](#important-notes)

## Game Overview
In this endless runner game, the player character moves horizontally from left to right (and potentially vertically up). The map and obstacles are generated procedurally and move toward the player, simulating forward movement.

The objective is to avoid incoming obstacles and keep running as far as possible. It's similar to the concept of **Hole in the Wall**, where you have to dodge objects and walls moving towards you.

## Tech Stack
- **OpenGL** for 3D rendering
- **[Unreal Engine](https://www.unrealengine.com/en-US)
 5** for game development
- **C++** for core game mechanics
- **Xcode** (for macOS users) or **Visual Studio** (for Windows users) as the IDE
- **GitHub** for version control

## Setup

### Cloning the Repository
To start working on this project, clone the repository to your local machine:

```bash
git clone https://github.com/SirKentut/endless-runner.git
```

### Unreal Engine Setup

1. Install Unreal Engine (minimum version 5.0 or later).
2. Open Unreal Engine.
3. Select **Open Project** from the file menu and locate the `EndlessRunner.uproject` file within the project directory.
4. Click **Open** to start working on the game.

### Build and Run

#### For macOS users:
1. Open **Xcode** and generate the project by navigating to `Source` → `EndlessRunner`.
2. Build the project by pressing `Cmd+B` or navigating to **Product** → **Build**.
3. Run the game using **Cmd+R**.

#### For Windows users:
1. Open the project using **Visual Studio**.
2. Ensure that all Unreal Engine plugins are properly installed.
3. Build and run the game via **Build Solution** in Visual Studio.

## Project Structure
```bash
├── Binaries/          # Binary files generated by Unreal Engine
├── Build/             # Build files for Unreal Engine
├── Config/            # Configuration settings
├── Content/           # Game assets, maps, and levels
├── Intermediate/      # Temporary build files
├── Source/            # C++ source files
│   ├── EndlessRunner/
│   │   ├── EndlessRunner.cpp          # Main game logic
│   │   ├── EndlessRunner.h            # Header for main game logic
│   │   ├── EndlessRunnerCharacter.cpp # Character-related code
│   │   ├── EndlessRunnerGameMode.cpp  # Game mode logic
│   │   ├── TP_PickUpComponent.cpp     # Component logic for item pick-ups
│   │   └── TP_WeaponComponent.cpp     # Weapon component logic
└── .gitignore         # Files to ignore in version control

```

## How to Contribute
### Working on the code

- Navigate to the `Source/EndlessRunner` directory.
- Open files like `EndlessRunnerCharacter.cpp` or `EndlessRunnerGameMode.cpp` to add or modify game logic.
- After making changes, follow the standard git flow to commit and push changes:

```bash
git add <file_name(s)> or "." 
git commit -m "Your commit message"
git push origin main
```

### Pull Requests (For now optional, high rec)
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`.
3. Make your changes.
4. Commit your changes: `git commit -m 'Add some feature'`.
5. Push to the branch: `git push origin feature-branch-name`.
6. Submit a pull request! 

## Important Notes

1. **Cross-Platform Collaboration:** This project is set up to be cross-platform. Both macOS and Windows users can work on the project. Make sure your teammates install the proper IDE and Unreal Engine version.

2. **File Generation:** Make sure not to commit files in directories like `Binaries/`, `Intermediate/`, or `Saved/`, as these are generated by Unreal Engine and should not be tracked by Git. These directories are excluded via `.gitignore`.

3. **Version Control:** Please follow the `git pull` → `git commit` → `git push` process to avoid merge conflicts.
