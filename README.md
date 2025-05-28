## Quantum ML Project: Exploring Quantum Mechanics with Deep Learning and Variational Monte Carlo
Project Overview
This project demonstrates an innovative approach to simulating and visualizing quantum mechanics phenomena using the power of Machine Learning. By combining Variational Monte Carlo (VMC) and Deep Neural Networks, we are able to approximate the wave functions of confined particles in different potentials and observe fundamental quantum behaviors, such as tunneling.

Furthermore, the project includes the architecture of a Variational Autoencoder (VAE), opening doors for future explorations in the generation and compression of quantum wave function representations.

Key Features
Potential Well Simulations: Implementation of simulations for:

Infinite Potential Well: A fundamental model for understanding quantum confinement and energy quantization.

Finite Potential Well: Demonstration of the Quantum Tunneling phenomenon, where a particle has a non-zero probability of existing in classically forbidden regions.

Wave Function Optimization with Neural Networks: Utilizes neural networks as variational wave functions, which are optimized to find the ground state (lowest energy) of the system.

Variational Monte Carlo (VMC): Employs the Metropolis-Hastings algorithm to sample the probability density of the wave function, allowing for the estimation of the system's energy and the optimization of the neural network parameters.

Interactive Visualization: Generation of plots that compare learned probability distributions with theoretical ones (where applicable) and illustrate wave function behavior.

Variational Autoencoder (VAE): Inclusion of a complete VAE architecture (Encoder, Decoder, VAE, and loss function) for future applications in:

Learning latent representations of wave functions.

Generating new wave functions or quantum states.

Dimensionality reduction for quantum data.

Technologies Used
Python: Primary programming language.

PyTorch: Deep Learning framework for building and training neural networks.

NumPy: For numerical operations and array manipulation.

Matplotlib: For visualization and plotting results.

How to Use
Prerequisites
Ensure you have Python installed (version 3.x recommended).
Install the necessary libraries via pip:

pip install torch numpy matplotlib

Execution
The main code for VMC simulations and the VAE definition are contained in Python files (or Jupyter cells, if you are using a notebook).

Clone the repository (if applicable):

git clone <YOUR_REPOSITORY_URL>
cd <your_repository_name>

Run the simulation script:
The main script (main.py or the name of your Python file containing the run_simulation and run_simulation_finite_well functions) contains the logic to train the models and generate the plots.

python main.py

Or, if you are using a Jupyter Notebook, execute the cells sequentially.

GPU Note: The code is configured to use GPU (CUDA) if available; otherwise, it will use the CPU. Monitor GPU usage (e.g., nvidia-smi in the terminal) to check for acceleration.

Expected Results
Upon running the project, you will be able to observe:

Probability Density Plots: Histograms of Monte Carlo samples that align with the probability density learned by the neural network.

Energy Convergence: Plots showing how the system's average energy decreases over training epochs, converging to the ground state value.

Tunneling Visualization: For the finite potential well, the plots will clearly demonstrate the "leakage" of the wave function outside the well's barriers.

Rejection Sampling (if implemented): A plot visualizing the accepted and rejected points during the sampling process.

Key Concepts
Wave Function (Ψ(x)): The mathematical description of a particle's quantum state.

Probability Density (∣Ψ(x)∣ 
2
 ): The probability of finding a particle at a given position.

Schrödinger Equation: The fundamental equation governing wave function behavior.

Potential Wells: Models of quantum confinement (infinite and finite).

Ground State: The lowest energy state of a quantum system.

Quantum Tunneling: The phenomenon where quantum particles can pass through potential barriers even without sufficient energy.

Variational Monte Carlo (VMC): A quantum simulation method that uses random sampling to optimize variational wave functions.

Neural Networks: Used as universal function approximators to represent wave functions.

Variational Autoencoder (VAE): A neural network architecture capable of learning latent data representations and generating new samples.

Next Steps and Future Extensions
This project provides a solid foundation for future explorations:

Excited States: Modify the model to find and visualize higher energy states (excited states).

Multiple Particles: Extend the simulation to systems with more than one particle, including interactions.

Higher Dimensionality: Adapt the model for 2D or 3D simulations.

VAE-VMC Integration: Explore how the VAE can be used to:

Generate trial wave functions for VMC.

Learn a latent space of VMC solutions to explore different quantum states.

Hyperparameter Optimization: Fine-tune training parameters (learning rate, Metropolis-Hastings step size).

Detailed Error Analysis: Implement methods like blocking to quantify the statistical uncertainty of energy results.

Author
Vittor Britis
