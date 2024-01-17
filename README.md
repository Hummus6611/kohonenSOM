# kohonenSOM
This Python code implements a Kohonen Self-Organizing Map (SOM) algorithm to cluster data points in a 2D space.
The SOM is trained on a given dataset, and the training process involves adjusting the weights of neurons to represent the input data distribution.

Here's a breakdown of the code:

Dataset:
Defines a 2D dataset containing data points with two features.

SOM Parameters:
W_Size: Size of the weight matrix, determining the number of neurons in the SOM.
alpha_0: Initial learning rate.
Epoch: Maximum number of training iterations.

SOM Initialization:
Initializes the weight matrix (W) with random values.

Training Loop:
Iterates through the specified number of epochs.
Randomly selects a data point from the dataset.
Determines the winning neuron by finding the one with the smallest Euclidean distance to the current data point.
Updates the weights of neurons based on the winning neuron's influence and the learning rate.

Learning Rate Decay Function:
Defines a function (alpha_decay) that decreases the learning rate over time.

Visualization:
Plots the SOM's weight vectors at specified intervals during training.
Neurons' positions in the 2D space are represented by markers, and each plot corresponds to a training step.

Result:
The final plot illustrates how the SOM has adjusted its neurons to represent the input data distribution.

The SOM learning process is visualized over multiple steps, providing insights into how the map evolves and adapts to the underlying structure of the data. The learning rate decay function contributes to fine-tuning the SOM's convergence over time.
