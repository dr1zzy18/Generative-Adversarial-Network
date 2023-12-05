MNIST GAN Project
Project Overview
This project is an implementation of a Generative Adversarial Network (GAN) trained on the MNIST dataset. It consists of a generator and a discriminator network that are trained adversarially to generate new, synthetic images of handwritten digits that resemble the real MNIST data.

Contents
gan.py: Main Python script implementing the GAN model.
MNIST_data/: Directory for storing the MNIST dataset.
MNIST_GAN_results/: Directory for storing output images and training history.
Requirements
Python 3.x
PyTorch
NumPy
Matplotlib
tqdm
torchvision
Installation
To install the necessary libraries, run the following command:


pip install torch numpy matplotlib tqdm torchvision
Dataset
The script will automatically download the MNIST dataset into the MNIST_data/ directory during the first run.

Running the Script
Execute the script by running:


python gan.py
This will start the training process. Generated images and loss plots will be saved in the MNIST_GAN_results/ directory.

Architecture
Generator
Input: Noise vector of dimension 100.
Output: Flattened image of dimension 784 (28x28 pixels).
Layers: Four fully connected layers with LeakyReLU activation (except the output layer which uses Tanh).
Discriminator
Input: Flattened image of dimension 784.
Output: Single value (probability of the image being real).
Layers: Four fully connected layers with LeakyReLU activation (except the output layer which uses Sigmoid).
Output
The training process will generate images at each epoch. These images, along with the loss history plot, will be stored in MNIST_GAN_results/.

Contributions
Contributions to this project are welcome. Please feel free to fork this repository, make changes, and submit pull requests.
