# Brick Breaker Meme

## Demo

Play the demo on Vercel using the following link: [Brick Breaker Meme - Demo](https://brick-breaker-meme-demo.vercel.app/)

---

## How to Play

- **Objective**: The player controls a paddle to keep the ball in play, aiming to destroy all bricks in the level. Some bricks require multiple hits to break.
- **Power-ups**: Activate special power-ups such as ball multiplication, fireball mode, and paddle expansion, which appear randomly during gameplay.
- **Audio-Visual Feedback**: The game adapts its visuals and sound effects based on player performance. If the player succeeds in destroying bricks, fun and joyful audio-visual cues appear. In case of failure, humorous "meme-style" animations and sounds are triggered.

---

## Features

1. **Power-up System**:
   - Special power-ups are available, including:
     - **BallsThree**: Multiplies the balls, adding more into the game.
     - **BigPaddle**: Expands the paddle, giving the player more control.
     - **FireBall**: Turns balls into fireballs that pass through bricks.
     - **AllBallsThree**: Introduces a larger number of balls for a chaotic and fun experience.

2. **Precise Collision and Physics**:
   - Balls and paddles use Godot’s `CharacterBody2D` and `move_and_collide` for accurate collision detection. Trajectories are adjusted based on the collision angle, ensuring responsive and dynamic gameplay.

3. **Ball Management**:
   - Ball mechanics include a multiplication feature that adds additional balls on screen. The script ensures global access to track game state, such as the number of active balls and their fireball state.

4. **Global Event System**:
   - Key game events, such as `multiply_all_balls`, `game_won`, and `game_lost`, are managed through a centralized global event system to keep gameplay synchronized and dynamic.

5. **UI and Level Navigation**:
   - The game features an intuitive user interface for navigating between levels and controlling game options, integrated with the global event system to manage transitions smoothly.

6. **Random Power-up Spawn**:
   - A probability system determines when power-ups appear, adding an element of surprise and strategy. Each destroyed brick has a chance to trigger a power-up, and power-ups spawn dynamically.

---

## Technologies and Concepts Used

1. **Godot Engine (GDScript)**:
   - The game is developed using Godot’s powerful 2D framework, with all core mechanics and features scripted in GDScript.

2. **Power-up System**:
   - Power-ups are modularly designed, with each power-up deriving from a base script to control its functionality, movement, and interaction with the player.

3. **Precise Physics and Collisions**:
   - Ball collisions are managed with `collision_normal`, ensuring that ball angles are calculated accurately based on impact.

4. **Audio-Visual Feedback**:
   - Dynamic audio and visuals respond to gameplay performance, creating an engaging, meme-driven experience.

---

## Future Improvements

- **New Power-ups**: Add more power-ups, such as speed boosts and ball shrinking.
- **Additional Levels**: Introduce more levels with increasing difficulty and variety in brick arrangements.
- **Mobile Optimization**: Optimize for touch controls and performance on mobile devices.

---

## License

The demo is for viewing purposes only.
