# Champion
Every day a worthy commit

# Hex-Based Top-Down Procedural Game

**Status:** In Development

**Language:** Python

**IDE:** VSCode (Windows)

**Genre:** Procedural Generation, Top-Down, RPG

## Overview

This project aims to create an engaging hex-based, top-down game with procedurally generated worlds. Players will explore a vast world filled with forests, hills, water bodies, settlements, and hidden dungeons. The game will feature turn-based combat, character progression, and a rich narrative.

## Core Features

* **Procedural Generation:**
    * Dynamically generate diverse 10x10 hex grids with varying terrain types (forest, open, hill, water, settlement).
    * Assign unique x,y coordinates to each hex for easy reference and interaction.
    * Populate hexes with content based on terrain (e.g., forests with trees, hills with resources).

* **Hex-Based Map:**
    * Utilize a hex map library (e.g., `hexmap`) to render the world as interconnected hexes.
    * Orient the grid with the flat side of the hex at the top for visual clarity.
    * Display artwork (`forest.png`, `hill.png`, etc.) in each hex to represent its type.
    * 1,500 ft. hexes, 750 ft. per side. 
    * Terrain type determines spotting distance in adjacent hexes.
    * 50% chance of a hex being the same type as the previous.

* **Character Classes & Equipment:**
    * Implement classes like Brute, Myrmidon, Rake, and Rogue, each with distinct attributes and starting equipment.
    * Champion is the starting class.
    * Assign armor class (AC), weapons, and gear based on character dexterity and class.
    * Implement class progression and equipment upgrades.

* **World Generation:**
    * Create a vast world filled with settlements, dungeons, and points of interest.
    * Populate settlements with lords and NPCs of varying levels.
    * 10% chance of town per hex, 1 hex per 6,000 people.
    * Generate dungeons with different themes (ruined settlements, castles, caves, etc.).
    * Implement terrain generation that impacts movement and exploration.

* **Turn-Based Combat:**
    * Design engaging turn-based combat mechanics.
    * Implement flanking mechanics for tactical combat.
    * Create a variety of monsters with different abilities and challenges.

## Development Plan (Python)

1.  **Hex Map Generation:**
    *   Use Python libraries like `numpy` or `pygame` to create the underlying hex grid data structure.
    *   Implement a procedural generation algorithm to fill the grid with terrain types based on the desired distribution.
    *   Store terrain data along with x,y coordinates in a dictionary or list.

2.  **Hex Map Rendering:**
    *   Research and choose a suitable hex map library (`hexmap` or similar).
    *   Load terrain artwork from the `./images` folder.
    *   Render the hex grid on the screen, placing appropriate artwork based on the terrain type in each hex.

3.  **Character Class Implementation:**
    *   Create Python classes (`Brute`, `Myrmidon`, etc.) to represent character classes.
    *   Define class attributes (AC, dexterity, equipment) and methods (attack, defend).
    *   Implement logic to assign starting equipment based on class and dexterity.

4.  **World Generation:**
    *   Develop algorithms to randomly generate settlements, dungeons, and points of interest.
    *   Populate the world with NPCs and assign them levels.
    *   Create a system for generating dungeon layouts and content.
    *   Consider using noise functions or other techniques for terrain generation.

5.  **Combat System:**
    *   Design a turn-based combat system with clear rules and mechanics.
    *   Implement actions like attack, defend, use items, and flee.
    *   Create monster classes with varying attributes and behaviors.
    *   Calculate damage, hit chances, and combat outcomes. 

## Additional Features (Future Development)

*   Multiplayer mode
*   Advanced crafting system
*   Character skill trees
*   More diverse enemy types and environments