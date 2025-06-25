This repository investigates the Ising model with the use of machine learning. 2D Ising models are generated at various temperatures which are then fed through a simple autoencoder. The 
autoencoder, as the name suggests, encodes these Ising systems into a two-neuron layer. This layer forms a 2D vector that is a part of a space known as the "latent" space in machine 
learning. This space reveals dominant behaviours of the systems due to the compression of information into the vector. What is found is that the vector serves as an order parameter to 
differentiate ordered vs. disordered systems across temperatures, and thus identify the critical temperature of the 2D Ising model. The graphs below display the heat map of the latent
space's 2D vectors (shown in the top graph), as well as the magnitudes of the 2D vectors and their susceptibility (i.e. variance of the 2D vectors' magnitudes), from which it is found that
the critical temperature is around 2.408. This result is not far off the analytical solution for the critical temperature of the 2D Ising model of approximately 2.269; hence, showing the
power of encoders in revealing hidden features from data. A better result could be achieved with a convolutional neural network autoencoder which would also train more rapidly. Doing so is left
as a possible future exercise.

![Output Graphs](https://github.com/user-attachments/assets/0f6425b9-da1d-4e2f-a540-90f89e3d335d)

This repository holds the autoencoder written from scratch (NumPy only) and with PyTorch. The NumPy-only autoencoder would take up too much computation time to train, and thus I didn't 
manage to get any results from it. Only the PyTorch autoencoder managed to train in a reasonable time, and hence provides results. Consequently, it seems best for personal projects
of mine, that I simply use PyTorch from the start.
