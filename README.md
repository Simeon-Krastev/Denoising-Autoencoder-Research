# Research on Denoising Autoencoders for Classification, Denoising, and Generation of MNIST Images

This is a PyTorch-based exploration of denoising autoencoders for a variety of tasks relating to the MNIST dataset.
As a start, the idea is to build a basic model that can do all three tasks given a specific kind of training. This will then be used as a starting point to research and mathematically model the boundaries between classes.

The project consists of the following exercises:

1. Building a basic linear layer Autoencoder to denoise MNIST images
2. Attempting to concatenate each MNIST image with a diffuse prior vector of all possible classes, and "Denoising" this diffuse prior to obtain a classification of the image
3. Exploring with an autoencoder that contains convolutional layers
4. Exploring adding noise before and after the first encoding
5. Using a classification approach where an image and a diffuse prior vector are input into the model, while the output consists of an image and the one-hot encoded label of the correspoding class
6. Using that same architecture, train the model for denoising
7. Attempt to train a model for both tasks at the same time
8. Add a third task, generation based on a given one-hot vector
9. Explore the capabilities of such a model
10. Explore training the model from scratch with inverted images
11. Compare this to training the model as before and fine-tuning the model with inverted images
12. Explore gradient descent on the input data to discover what the model understands under each class, and represent the boundaries between classes as homotopies
