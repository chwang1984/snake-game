# Snake Game - HTML5 Canvas

## Project Overview
- **Type**: Classic arcade game
- **Core**: Snake game with retro neon aesthetics
- **Target**: Desktop and mobile browsers

## Visual Specification

### Canvas Setup
- Responsive canvas scaling to fit viewport
- Grid-based game board (20x20 cells)
- Cell size calculated dynamically

### Color Palette
- Background: #0a0a0a (near black)
- Grid lines: #1a1a2e (subtle)
- Snake head: #00ff88 (neon green)
- Snake body: #00cc6a (darker green gradient)
- Food: #ff4757 (neon red/pink)
- Score text: #ffffff
- Glow effects: box-shadow/canvas shadow

### Typography
- Font: "Press Start 2P" (Google Fonts) - retro pixel style
- Fallback: monospace

## Game Specification

### Snake Mechanics
- Initial length: 3 segments
- Initial position: center of grid
- Initial direction: right
- Speed: 150ms per move (adjustable)

### Movement
- Arrow keys / WASD for direction
- Cannot reverse direction (no 180° turns)
- Continuous movement in current direction

### Food Generation
- Random position on grid
- Never spawns on snake body
- New food spawns after consumption

### Collision Detection
- Wall collision: game over
- Self collision: game over

### Scoring
- +10 points per food
- High score stored in localStorage

## Interaction Specification

### Controls
- Arrow keys: direction control
- WASD: alternative direction control
- Space/Enter: start/restart game
- P key: pause/resume

### Game States
- START: Title screen with instructions
- PLAYING: Active gameplay
- PAUSED: Game paused overlay
- GAMEOVER: Game over with score display

## Responsive Design
- Canvas scales to fit container
- Maintains aspect ratio
- Touch controls for mobile (swipe gestures)
- Minimum playable size: 300x300px

## Acceptance Criteria
1. Snake moves smoothly in all 4 directions
2. Food appears randomly and snake grows when eating
3. Game ends on wall or self collision
4. Score displays and updates in real-time
5. High score persists across sessions
6. Game restarts on keypress after game over
7. Responsive on different screen sizes
8. Touch/swipe controls work on mobile
