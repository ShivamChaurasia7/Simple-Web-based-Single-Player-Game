# Simple-Web-based-Single-Player-Game

# Car Dodging Game

A simple car dodging game where the player controls a car using the keyboard to avoid traffic. The objective is to survive as long as possible, with the score increasing based on the distance traveled or time survived. The game ends if the player's car crashes into another car, displaying a game-over screen with the final score and an option to restart.

## User Stories

1. **Start the Game**
    - **As a Player, I want to start the game, so that I can begin playing.**
        - Acceptance Criteria:
            - There should be a start button on the main screen.
            - Clicking the start button initiates the game.

2. **Control the Car**
    - **As a Player, I want to control the car using my keyboard, so that I can avoid traffic.**
        - Acceptance Criteria:
            - The car can be moved using W for up, A for left, D for right, S for down arrow keys.
            - The car movement should be smooth and responsive.

3. **Track Score**
    - **As a Player, I want to see my score increase as I dodge traffic, so that I can track my progress.**
        - Acceptance Criteria:
            - The score increases based on the distance traveled or time survived.
            - The current score is displayed on the screen.

4. **Avoid Crashing**
    - **As a Player, I want to avoid crashing into other cars, so that I don't lose the game.**
        - Acceptance Criteria:
            - Crashing into another car ends the game.
            - A game-over screen is displayed with the final score and an option to restart.

5. **Game Over Screen**
    - **As a Player, I want to see a game-over screen when I lose, so that I know the game has ended.**
        - Acceptance Criteria:
            - The game-over screen displays the final score.
            - There is a restart button to play the game again.

6. **Restart the Game**
    - **As a Player, I want to restart the game after it ends, so that I can play again.**
        - Acceptance Criteria:
            - Clicking the restart button restarts the game from the beginning.

## Data Models

### Player
- **Attributes:**
    - `score`: integer, keeps track of the player's current score.
    - `isGameOver`: boolean, indicates whether the game has ended.

### Game Object
- **Attributes:**
    - `type`: string, indicates the type of object (e.g., 'car').
    - `positionX`: number, the current X position of the object.
    - `positionY`: number, the current Y position of the object.
    - `speed`: number, the speed at which the object moves.

### Car
- **Attributes:**
    - `positionX`: number, the current X position of the car.
    - `width`: number, the width of the car.

## Example Game Flow

1. **Start Screen:**
    - Display a start button.
    - Player clicks start to begin the game.

2. **Game Play:**
    - Player’s car drives forward and traffic cars move towards the player from the top of the screen.
    - Player moves the car left and right to avoid traffic.
    - The score increases based on the distance traveled or time survived.
    - If the player's car crashes into another car, the game ends.

3. **Game Over:**
    - Display the final score.
    - Show a restart button.
    - Player clicks restart to play again.

## Technologies

- **HTML5**: Structure of the game.
- **CSS3**: Styling and animations.
- **JavaScript**: Game logic and interactivity.
- **Game Development Library (Optional)**: Libraries such as Phaser.js for easier game development and handling animations.

## Implementation Plan

1. **Setup Project:**
    - Create the basic HTML structure.
    - Add CSS for styling the game elements.
    - Initialize a JavaScript file for game logic.

2. **Create Game Elements:**
    - Car element that can be moved left and right.
    - Traffic car elements that move from the top to the bottom of the screen.

3. **Implement Game Logic:**
    - Handle user input to move the car.
    - Create functions to randomly generate traffic cars.
    - Check for collisions between the player’s car and traffic cars.
    - Update the score based on the distance traveled or time survived.
    - End the game when a collision occurs.

4. **Add Animations and Interactivity:**
    - Use CSS animations for smooth car movements.
    - Add interactive UI elements for starting and restarting the game.

5. **Testing and Refinement:**
    - Test the game for responsiveness and smooth gameplay.
    - Make adjustments to game difficulty and visual appeal.
