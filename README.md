# TV Script Generation


## What is this project?

In this project, I generated my own Seinfeld TV scripts using RNNs. I used part of the Seinfeld dataset of scripts from 9 seasons. The Neural Network I built generates a new ,"fake" TV script, based on patterns it recognizes in this training data.

## Stages of the project:

1. Get the Data.
2. Explore the Data.
3. Implement Pre-processing Functions.
   - Lookup Table.
   - Tokenize Punctuation.
4. Build the Neural Network.
   - Input as batches.
   - The neural network that have been trained is `lstm`.
5. Training the neural network
   - Hyperparameters choosing.
6. Generate new TV Script based on trained network.


## Note:

The project is a part of Deep Learning Nanodegree, [here](https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-tv-script-generation)
