# 1. Image Classification with CNN and CIFAR-10 Dataset
## Convolutional Neural Network (CNN):

- Purpose: CNNs are used primarily for image classification tasks. They can automatically and adaptively learn spatial hierarchies of features from input images.
- Architecture:
1. Convolutional Layers: Apply convolution operations to the input image, using filters to detect various features like edges, textures, and patterns.
2. Pooling Layers: Reduce the spatial dimensions of the feature maps, retaining essential information while reducing computation.
2. Fully Connected Layers: Serve as the classifier, taking the flattened feature maps and outputting class probabilities.
- Key Techniques: Data augmentation, dropout for regularization, and using softmax for classification.

# 2.Detect Computer Security Breach using RNNs and LSTMs
## Recurrent Neural Network (RNN):

- Purpose: RNNs are designed to handle sequential data and time series data by maintaining a hidden state that captures information from previous time steps.
- Architecture:
1. Recurrent Layers: Use loops within the network to process sequences of inputs, maintaining hidden states.
2. Issues: RNNs can suffer from vanishing and exploding gradient problems, making them less effective for long sequences.

## Long Short-Term Memory (LSTM):

- Purpose: LSTMs are a type of RNN that are capable of learning long-term dependencies. They address the vanishing gradient problem through their unique architecture.
- Architecture:
1. Cell State: A key component that runs through the entire LSTM, enabling the network to maintain and modify the memory.
2. Gates:
2-1. Forget Gate: Decides what information to discard from the cell state.
2-2. Input Gate: Decides which values from the input to update the cell state.
2-3. Output Gate: Decides what to output based on the cell state and the current input.
- Application: Used for anomaly detection by learning the normal patterns in sequential data and identifying deviations from these patterns.

# 3. Generate New Picture using VAE
## Variational Autoencoder (VAE):

- Purpose: VAEs are generative models that learn to encode input data into a latent space and then decode it back to the original input space. They are used for generating new data samples similar to the training data.
- Architecture:
1. Encoder: Compresses the input data into a latent space representation.
2. Latent Space: Represents the compressed data as a distribution (mean and variance).
3. Decoder: Reconstructs the data from the latent space representation back to the original data space.
- Key Techniques:
1. Reparameterization Trick: Allows gradient descent to be used for training by introducing stochasticity in the latent space.
2. Loss Function: Combines reconstruction loss (how well the output matches the input) and KL divergence (difference between the learned latent space distribution and a prior distribution).
