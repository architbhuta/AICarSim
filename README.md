

---

# Car Simulation using NEAT and Pygame

This project simulates autonomous cars learning to navigate a track using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm. The cars evolve over generations, improving their navigation capabilities through reinforcement learning and genetic algorithms.

## Table of Contents
- Project Overview
- Getting Started
- Prerequisites
- Installation
- Running the Simulation
- Project Structure
- How it Works
- License

## Project Overview
The simulation showcases autonomous cars using a neural network controlled by the NEAT algorithm to navigate a map. The cars are equipped with virtual radar sensors to detect distances to track borders. By evolving over generations, the cars learn to improve their performance.

## Getting Started
Follow these instructions to set up and run the project on your local machine.

### Prerequisites
- Python 3.x
- `pygame` library
- `neat-python` library

### Installation
1. Clone this repository:
   ```
   git clone https://github.com/your-username/car-simulation-neat.git
   cd car-simulation-neat
   ```
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Make sure you have `car.png` (the car sprite) and `map2.png` (the map image) in the project directory.

### Running the Simulation
Run the following command to start the simulation:
```
python main.py
```

## Project Structure
- `main.py`: The main script containing the simulation logic.
- `car.png`: Image file representing the car.
- `map2.png`: Map image for the simulation track.
- `config.txt`: Configuration file for the NEAT algorithm.
- `README.md`: Documentation file.

## How it Works
### NEAT Algorithm
- NEAT (NeuroEvolution of Augmenting Topologies) evolves neural networks using genetic algorithms.
- Neural networks are controlled by genomes, which mutate and evolve over generations based on fitness scores.

### Car Behavior
- The cars start at a fixed position and try to navigate the track.
- The cars receive radar data (distances to borders) and use a neural network to decide actions (turning, speeding up, slowing down).
- Fitness is determined by how far each car travels without colliding.

### Pygame for Rendering
- `pygame` handles graphical rendering, drawing the map, cars, and radar sensors.

