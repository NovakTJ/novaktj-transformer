# novaktj-transformer
**A decoder-only transformer, similar to GPT.**
I created a transformer model from scratch, using only PyTorch and a tokenizer. The code is a replication of 'Attention is all you need'.

I implemented:
1. Positional embedding
2. Multi-head attention
3. Training code

I also made unit tests and a toy task to quickly test model variations. 

The dataset is currently too small - I did not augment the data - and the training is over in about a minute on a Colab free GPU. After training, the model usually converges on predicting a space every time.

Note from a year later: it seems that i did backprop only from the last token, making the training 50x less efficient.

I'll come back to this project!
