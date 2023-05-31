# AI-FOR-HACKING

## A simple Bigram model to predict the next token in the given sequence

- The model takes in a series of tokenized characters and outputs the next predicted characters in the sequence.
- Model can be modfied to predict n number of tokens together which would help increase speed but would however result in meaningless generation as accuracy drops drastically.
- A single token is generated and the next resulting generation is fed back into the model recursively until maximum length is exceeded or a termination token is encountered.


## Architecture
The bigram model is based on the transformer acrhitecture which can be visualised as follows

![image](https://github.com/devesh2003/AI-FOR-HACKING-ILGC/assets/43497480/a490b4d1-7f81-4641-bb89-306db6db1e97)

The transformer typically consists of 2 main components 
1. Encoder
2. Decoder

Our model only uses the decoder for faster and more efficient generation. In the current scenario encoder block can be ignored as we don't need context specific generation of sequences but instead require generation based on the current OUTPUT context.

In-depth and detailed explaination of the decoder architecture and attention mechanism in the notebook itself.
