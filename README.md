# BomberQuest

**A 2D maze adventure built with Java and libGDX**

Java 17 · libGDX · Gradle · Object-Oriented Programming

## Overview

BomberQuest is a Bomberman-inspired, 2D tile-based game set in a foggy forest maze. Players navigate destructible environments, battle ghosts and slimes, collect power-ups and defeat a final boss to unlock the hidden exit before time runs out.

Developed as a two-person university project for *Introduction to Programming* at the Technical University of Munich (WS 2024/25).

## Gameplay

Players can choose from five preloaded levels, load a custom map or play together in local two-player mode. Each level combines destructible obstacles, hidden power-ups, enemy encounters and a countdown timer.

## Key features

### Enemy AI and boss encounters
- Slimes move randomly and change direction when blocked.
- Ghosts pursue players within their visible range and otherwise move randomly.
- A skeleton boss appears after all other enemies are defeated. It has three lives and temporary invincibility after taking damage.

### Dynamic fog of war
Players can only see seven tiles in each direction. The visible area moves with the player, concealing enemies and obstacles beyond that range.

### Local multiplayer
Two players can play on the same keyboard using separate controls while sharing lives and power-ups.

### Custom maps and level progression
The game can load external map files and includes five preloaded levels of increasing difficulty. Maps without a predefined exit automatically receive one beneath a randomly selected destructible wall.

### Scoring and persistent highscores
Players earn points for eliminating enemies, defeating the boss, completing levels and finishing with time remaining. The five highest scores are stored in a file and displayed in the game.

### Dynamic countdown
The timer begins at 2:30, with 15 additional seconds for every initial enemy. Defeating all regular enemies triggers the boss encounter and awards 30 additional seconds.

### Power-ups
Players can collect upgrades to increase the number of simultaneous bombs, extend the explosion radius or gain an extra life.

## Technical architecture

The game uses object-oriented programming and separates gameplay logic, rendering, audio and screen management.

| Component | Responsibility |
|---|---|
| GameMap | Map loading and updates |
| CollisionDetector | Collision detection and responses |
| GameObject | Base class for game entities |
| Enemy | Base class for enemy types |
| Screen classes | Menus, gameplay, pause and end screens |
| PointReader | Persistent high-score management |



## Gameplay screenshots

<img width="959" height="539" alt="Screenshot 2026-09-25 133637" src="https://github.com/user-attachments/assets/106df689-d47b-4051-8114-46e927d735c2" />
<img width="959" height="539" alt="Screenshot 2026-09-25 133637" src="https://github.com/user-attachments/assets/60102d76-b69c-42f5-9d3a-902a1c012f0f" />


## Source code

The source code is not currently public while permission to publish the original university project is being clarified.

## Acknowledgements

Developed as a two-person group project for Introduction to Programming at TUM (WS 2024/25), using a course-provided starter template. Third-party assets and contributors will be credited as appropriate.
