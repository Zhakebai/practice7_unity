# Practice 8-9 pygame
# Maze Shooter Game

## Overview

Maze Shooter Game is a 2D tile-based game built with Pygame. The game features a procedurally generated maze where you, as the hero, navigate corridors, avoid hazardous lava, and battle horizontally moving enemies. With each level, the challenge increases as more lava is added and enemy tactics keep you on your toes.

## Features

- **Procedural Maze Generation:**  
  Uses a recursive backtracking algorithm to generate maze layouts with walls and open corridors.

- **Dynamic Lava Placement:**  
  Lava is placed only on "central" corridor tiles.  
  - Level 1: 5 lava tiles  
  - Each subsequent level: +2 lava tiles  
  Lava is drawn using a transparent image that covers the entire tile.

- **Player Mechanics:**  
  - **Movement:** Use **W**, **A**, **S**, **D** to move.  
  - **Jumping:** Press **J** to jump to the next safe tile (skipping over lava).  
  - **Shooting:** By default, the hero shoots to the right. Changing direction causes the hero to shoot in that new direction. Use **SPACE** to shoot.

- **Enemy Behavior:**  
  - **Movement:** Enemies move only horizontally. They chase the hero when close and wander randomly when far. They check the tile ahead; if blocked, they reverse direction.
  - **Shooting:** Enemies shoot horizontally when the hero is in the same row and on the side they are facing, provided there’s a clear line-of-sight.

- **Camera Scrolling:**  
  Smooth camera scrolling follows the hero throughout the maze.

- **Restart Option:**  
  After a win or game over, a restart screen is displayed. Press **R** to restart the game.

- **Sound & Music:**  
  The game includes sound effects for actions (click, shoot, jump) and background music.

## Installation

**Prerequisites:**  
   - Python 3.x  
   - Pygame (install with `pip install pygame`)
   - 
## Assets

Make sure the following files are in your project directory:
- **hero.png** – Sprite for the player.
- **enemy.png** – Sprite for the enemies.
- **lava.png** – Image used for lava tiles (with transparency).
- **click.wav** – Sound effect for mouse clicks.
- **shoot.wav** – Sound effect for shooting.
- **jump.wav** – Sound effect for jumping.
- **background.mp3** – Background music.

Controls
W, A, S, D: Move the hero.
SPACE: Shoot in the hero’s current facing direction (default is right).
J: Jump to the next safe tile in the direction the hero is facing (skips over lava).
R: Restart the game after a win or game over.

**How It Works
Maze Generation
A recursive backtracking algorithm creates a maze where walls are represented by # and passages by .. The maze provides the grid structure for the game
