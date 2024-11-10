# Snake Game AI

This project implements a Snake game AI using Deep Q-Learning. The AI learns to play the Snake game by training a neural network to predict the best moves.

## Project Structure

- `agent.py`: Contains the `Agent` class that interacts with the game and trains the neural network.
- `helper.py`: Contains helper functions for plotting the training progress.
- `model.py`: Contains the neural network model (`Linear_QNet`) and the trainer class (`QTrainer`).
- `snake_game.py`: Contains the `SnakeGameAI` class that implements the Snake game logic.

## Requirements

- Python 3.x
- PyTorch
- NumPy
- Matplotlib
- Pygame

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/snake-game-ai.git
    cd snake-game-ai
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

To train the AI, simply run the `agent.py` script.

## How It Works

- **Game Environment**: The `SnakeGameAI` class in `snake_game.py` handles the game logic, including movement, collision detection, and food placement.

- **Agent**: The `Agent` class in `agent.py` interacts with the game environment. It uses a neural network to predict the best moves based on the current state of the game.

- **Neural Network**: The `Linear_QNet` class in `model.py` defines a simple feedforward neural network with one hidden layer. The `QTrainer` class handles the training process using the Q-learning algorithm.

- **Training**: The `train` function in `agent.py` runs the training loop. It collects game states, actions, rewards, and next states, and uses this data to train the neural network.

## Note

This project was built with the help of a tutorial. You can find the tutorial on [YouTube](https://www.youtube.com/watch?v=L8ypSXwyBds&list=PLwwsZ1mqtU_jPiIFV9TBe3V5ejO4oNqDW).