# NMT
Here I will put different variation of NMT models, as I implement them

# Libraries
* Pytorch 1.7
* Torchtext 0.8.0

# A seq2seq NMT model without attention

The first model is a simple seq2seq model that does not have attention layer. The encoder is a GRU network, and the decoder is also a GRU network.
To train the network I use teacher forcing technique, in this way that for each batch it decides randomly that what should be the input to the decoder?
Should it be the gold-standard traget token, or should it uses the network prediction from the previous time step?

