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

## Hyperparameters:

```py
:
# Data params
# Sequence Length
sequence_length = 12  # of words in a sequence
# Batch Size
batch_size = 64

# data loader - do not change
train_loader = batch_data(int_text, sequence_length, batch_size)


# Training parameters
# Number of Epochs
num_epochs = 10
# Learning Rate
learning_rate = 0.001

# Model parameters
# Vocab size
vocab_size = len(vocab_to_int)
# Output size
output_size = vocab_size
# Embedding Dimension
embedding_dim = 500
# Hidden Dimension
hidden_dim = 600
# Number of RNN Layers
n_layers = 3

# Show stats for every n number of batches
show_every_n_batches = 500
```

## Generated text: 

```txt
elaine: announcer frog mouths opened up the window.

george:(pleading) what?

jerry: well, i don't want to hear it.

kramer:(indicating) well, i got it. i was just wondering what i'm gonna tell you, i can't get it out of here.

kramer: well, i don't know how you feel.

jerry: you don't know, i can't. but i don't think we are gonna do it. i don't have any furniture.

elaine: i know, but i can't help her.

elaine: i don't want to talk to him, but...

jerry: oh yeah...

george: you know, i've been thinking about it, jerry. i just came in. i got to go out with him.

jerry:(to the phone) yeah.

kramer: hey, hey! you know i got a hopper?

jerry: yeah, yeah.

elaine: what is that about?

jerry: what? why?

george: well, you know the point of the post office. the spit of the aryan union. the horror, they have no choice. the only way you know, i think he's in the hospital. i just wanted you to know me.

elaine:(leaving) i know, but it's a good thing.(jerry picks it up)

george: so, what do you think? you think she thinks he was a maid?

jerry: he didn't get
```

## Note:

The project is a part of Deep Learning Nanodegree, [here](https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-tv-script-generation)
