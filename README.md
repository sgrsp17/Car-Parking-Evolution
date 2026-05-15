# Blackjack Neuroevolution Agent (BIAI)

## Overview
This project implements an Artificial Intelligence agent designed to play the Blackjack environment provided by Gymnasium (`Blackjack-v1`). The core objective is to develop a robust neural network controller trained via neuroevolution, specifically utilizing a Genetic Algorithm for global optimization.

## Project Structure
- `environment.py`: Manages the integration with the Gymnasium `Blackjack-v1` environment. It handles state observation retrieval, action execution, and the rendering lifecycle.
- `main.py`: The designated entry point for orchestrating the neuroevolution training process and agent evaluation.
- `neural_network.py`: Contains the architecture and forward-pass logic for the neural network controller that determines the agent's actions based on environmental states.

## Setup and Dependencies
Ensure a compatible Python version (3.13 is recommended) is installed. The environment requires the following core dependencies:

```bash
pip install gymnasium numpy
```

*Note: For graphical rendering using `render_mode="human"`, the `pygame` package is additionally required.*

## Usage
To test the core environment functionality and the action loop, execute:

```bash
python environment.py
```

This will initialize the Blackjack environment, execute a sample action loop, and display the resulting observation states (Player's sum, Dealer's showing card, Usable Ace indicator) and step rewards in the console. The environment window will cleanly exit after a 3-second delay upon game completion.
