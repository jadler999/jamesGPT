# Bigram Language Model

This Python script implements a simple Bigram Language Model using PyTorch. The model is based on the architecture proposed in the paper Attention is All You Need.
## Overview

The Bigram Language Model is designed to predict the next character in a sequence of text based on the previous character. It utilizes a transformer architecture, specifically multi-head self-attention, to capture dependencies across the input sequence.

## Usage

1. **Dependencies**: Make sure you have PyTorch installed. You can install it via `pip install torch`.

2. **Input Data**: Prepare your text data and save it in a file named `message_log.txt`.

3. **Hyperparameters**: Adjust hyperparameters such as batch size, block size, and learning rate according to your requirements.

4. **Training**: Run the script to train the model. It will print the training and validation loss at regular intervals.

5. **Generation**: After training, the script will generate text based on the learned patterns. The generated text will be printed to the console.

## Model Architecture

The Bigram Language Model consists of the following components:

- **Token Embedding Table**: Embeds input tokens into a continuous vector space.
- **Position Embedding Table**: Encodes positional information of tokens.
- **Multi-Head Self-Attention Blocks**: Process input tokens in parallel, capturing dependencies.
- **FeedForward Networks**: Apply non-linear transformations to the output of attention blocks.
- **Layer Normalization**: Normalize outputs of each block to stabilize training.
- **Linear Output Layer**: Maps the final embeddings to logits for next character prediction.

## Credits

Credit to Andrej Karpathy and his Makemore series which this model draws from. 

## Author

This Python script was authored by James Adler. Feel free to reach out with any questions or suggestions.
