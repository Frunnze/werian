# Werian

## Tasks
### Phase 1: Project Setup and Core Systems
#### 1. Set Up Project Environment
- Initialize a Pygame project with essential folders for assets (images, sounds), scripts, and data.
- Implement a GameManager class using the Singleton Pattern to handle game state and resource management.

#### 2. Create Base Classes for Game Objects
- Develop a base GameObject class for all in-game entities (enemies, towers, UI elements).
- Define a Sprite handling system for efficient asset rendering.

#### 3. Implement Core Game Loop
- Establish a basic game loop for rendering, updating, and processing player input.

#### 4. Resource Management System
- Create a resource system within GameManager to handle point allocation, upgrades, and overall game economy.

### Phase 2: Tower and Enemy Factories (Factory Pattern)
#### 5. Design Tower and Enemy Factories
- Implement TowerFactory and EnemyFactory classes using the Factory Pattern to create specific towers (Archer, Mage) and enemies (Goblin, Orc) on demand.

#### 6. Develop Base Tower Class
- Create a Tower base class with core attributes (damage, range, attack speed) and methods for placement, upgrading, and attacking enemies.

#### 7. Implement Specific Towers
- Develop ArcherTower and MageTower subclasses, with specific attributes and abilities (e.g., Archer for fast attacks, Mage for area damage).

#### 8. Define Tower Placement Mechanic
- Implement grid-based tower placement logic allowing towers to be placed only on designated tiles.
- Add cost requirements for tower placement and upgrade.


### Phase 3: Enemy Wave System
#### 9. Create Enemy Base Class
- Define an Enemy base class with attributes like health, speed, and reward points for player kills.

#### 10. Develop Basic Enemy Types
- Implement Goblin and Orc subclasses with unique attributes (e.g., Orc has higher health, Goblin is faster).

#### 11. Implement Enemy AI
- Develop pathfinding logic for enemies to follow towards the castle, accounting for obstacles and towers.

### 12. Create Wave System
- Implement a wave manager to spawn enemies in waves of increasing difficulty.
- Develop a countdown timer and spawning logic for each wave, managing enemy attributes (e.g., speed, health) per wave.


### Phase 4: Boss Enemies and Special Enemy Behaviors
#### 13. Design Boss Enemy Class
- Create a BossEnemy class with increased health, special abilities, and an area of effect (AoE) heal/shield for nearby enemies.

#### 14. Implement Boss Abilities
- Develop abilities for the boss, such as healing other enemies within range or activating a shield.

#### 15. Add Strategy Pattern for Enemy Behaviors
- Implement the Strategy Pattern for enemy AI to change behaviors, allowing enemies to adapt to player actions (e.g., path avoidance if close to high-damage towers).

### Phase 5: Tower and Enemy Interactions (Observer Pattern)
#### 16. Implement Observer Pattern for Enemy Detection
- Use the Observer Pattern to allow towers to detect enemies within range and initiate attacks.

#### 17. Enemy Health and Damage Handling
- Implement a damage system for towers to reduce enemy health and track kill rewards.
- Add animations and sound effects for attacks and enemy deaths.

### Phase 6: UI and Game Mechanics Integration
#### 18. Develop Core User Interface
- Implement the main HUD with real-time displays for castle health, player points, and wave status.

#### 19. Create Tower Placement and Upgrade UI
- Add a selection menu for available towers with placement and upgrade costs.
- Implement click interactions for tile selection, tower placement, and tower upgrades.

#### 20. Implement Wave Tracker UI
- Add a wave tracker displaying countdown, wave progress, and a preview of upcoming enemy types.

#### 21. Economy and Resource System
- Implement point management for earning points through enemy kills, and use points to place or upgrade towers.

#### 22. Game Over and Victory Screens
- Develop a game-over screen with a summary of enemies defeated, points earned, and towers built.
- Create a victory screen to display the player's success upon defending all waves.


### Phase 7: Visual and Audio Enhancements
#### 23. Integrate Visual Assets
- Add visual assets (sprites) for towers, enemies, the castle, and UI components for visual clarity.

#### 24. Implement Sound Effects
Add sound effects for tower attacks, enemy deaths, and UI interactions (e.g., placement, upgrade clicks).


### Phase 8: Advanced Mechanics and Final Touches
#### 25. Enhance Boss AI with Notifications
- Refine Boss AI so that it can notify nearby enemies for AoE effects (healing or shielding).

#### 26. Implement GameManager Level Controls
- Use GameManager to manage level transitions, resource resets, and game state checks for wave transitions.

#### 27. Fine-Tune Game Balancing
- Adjust health, damage, speed, and costs for towers and enemies to ensure fair difficulty progression across waves.

#### 28. Optimize Performance
- Implement optimizations for efficient rendering, collision detection, and event handling to improve game performance on PC.


### Phase 9: Final Integrations and Build
#### 29. Finalize All Game Assets
- Ensure that all sprites, sound files, and UI assets are correctly assigned and loaded within the game.

#### 30. Prepare Game for Build
- Integrate all final game elements, validate asset loading, and create a build script for packaging the game for PC deployment.


## Resources
Presentation pitch - [link](https://docs.google.com/presentation/d/1GRjH5aPtyEq99QnvBUe6jkKHB1lA4dbhHLqISl9yxjI/edit?usp=sharing)<br>
Technical Documentation - [link](https://docs.google.com/document/d/103_Ir860kYcKOXY2BoJTDCFr6X6eIhuD6F3l1olw7KI/edit?usp=sharing)
