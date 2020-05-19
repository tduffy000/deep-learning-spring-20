## Fundamentals of ML with NN
1. We want to build an autoencoder with a squeeze layer in the hidden dimension that will project our input features to a smaller latent space so we can use those embeddings as features themselves. Here, we are attempting to perform:
- **Dimension reduction**
- Supervised learning
- Reinforcement Learning
- Regularization

2. We call $L_1$ and $L_2$ regularization, respectively:
- Ridge and Lasso
- Norm and Binorm
- **Lasso and Ridge**
- Least Squares and LOESS

## Convnet Deep Learning Computer Vision

1. How can we use a pre-trained classifier (like VGG16) trained on an entirely different dataset relevantly in our custom classification problem?
- By copying the architecture are training it on our dataset just changing the input size
- By adding the dataset that model was trained on to ours and training it on their union.
- **By using the weights of the convolution layers as feature mappings and adding our own fully connected network on top.**
- We shouldn't it's not really relevant.

2. Which one of the following is *not* a viable data augmentation technique for images?
- Vertically flipping images.
- Rotating the images a random number of degrees.
- Fluctuate the RGB intensities of images.
- **Remove certain images from our training set.**

## RNN and working with Text

1.

2.
    Tokens: Letters, words, n-grams
    Bag of words
    One hot encoding
    Word Embeding, eg. Word2Vect, GloVe (pretrained) similarity
    Skipgram vs CBOW (Word2Vect)
    SimpleRNN
    LSTM and GRU
    Time Series
    Comparing with Baseline model
    Stacked Recurrent Layers
    Bidirectional
    1-D Convnet approach
    CNN+ Convnet
    Attention (Neural Touring Machine, etc)
    Transformers
    Bert

## Advanced Deep Learning Practices

    Keras functional API
    Multi-input Model
    Multi-output Model
    Vanishing Gradient Problem
    Layer Weight Sharing
    Models as Layers
    Model Checkpointing
    Dearly Stopping
    Logging
    Tensor Board (what it is, what can it do)
    Batch Normalization
    Hyperparameter Optimization
    Model Ensembling

## Generative Networks

1. GANs were motivated by which of the following concepts / algorithms from Game Theory
- **Minimax**
- Nash's algorithm
- Goodman's algorithm
- Expectimax

2.


    Generative RNN (generating sequence data)
    Greedy vs Stocastic Sampling and “temperature”
    DeepDream network
    Gradent assent (input)
    Neural style transfer
    Content loss vs style loss
    Autoencoders
    Variational Autoencoders
    Latent spaces
    Generative adversarial networks
    DCGAN (Deep Convolutional Network)
    StyleGAN 1
    StyleGAN 2
    Pix2Pix
    CycleGan
    Deep Fakes (classical vs DNN)
    Adversarial Examples
    Adversarial Attacks (White box vs Black Box)
    Adversarial Examples on Humans
    Adversarial examples as a feature (rather than a bug)

## Reinforcement Learning

1. A Markov chain / process has *this* particular property with respect that relates $P(X_{t+1} | X_t)$ and $P(X_{t+1} | X_{t-1} )$
if our current state is $t$:
- **The state of the system at $t-1$ is irrelevant at $t$ w.r.t probability of $t+1$**
- It is monotonically increasing as a function of $t$
- It says that we can no longer return to the state of the system at $t-1$ from $t+1$
- It is saturating

2.

    Agent vs. Envirionment
    States, Action, Reward
    Dynamics of Environment
    Model-based vs Model Free
    Markov process
    Episodic vs Continuous
    Short-term Reward vs Long Term Return
    Discount Rate
    Policy
    Value of a Policy
    Q-function
    Bellman Equation
    Dynamic Programing for Reinforcement Learning
    Monte Carlo for Reinforcement Learning
    Explore and update (greedy)
    Temporal Diffences
    Off Policy vs. On Policy
    Deep Q-learning
    Deep Q-Network
