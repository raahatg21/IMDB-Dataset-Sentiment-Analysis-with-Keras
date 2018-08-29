# IMDB-Dataset-Sentiment-Analysis-with-Keras

  Sentiment Analysis is done on IMDB Dataset that comes bundled with Keras. It consists of 25,000 training samples (of which 20% are validation) and 25,000 test samples. All words in the dataset are pre-tokenized. Self-trained word embeddings are used (the Keras Embedding layer).
  
  I've trained two models, the first of which (IMDB_RNN_1.ipynb) contains of a single **LSTM layer**. It gives **87.9% accuracy** on 15 epochs. The second example (IMDB_RNN_2.ipynb) consists of 2 sets of **Conv1D** and **MaxPooling1D** layers followed by standard **GRU layer**. **85.34% accuracy** is observed.
  
  I've used **CuDNN** layers for LSTM and GRU as they are much faster on GPU than standard LSTM and GRU layers. Recurrent dropout is not available with CuDNN, hence not used. https://github.com/keras-team/keras/issues/8935
  
  All implementations are made using **Keras**. This example was inspired by the book **Deep Learning with Python** written by Keras author Francois Chollet. 
  
  The files are created in Google Colab. Link is included.
  
  Comments and Suggestions are welcome :)
  
  Author: Raahat Gupta
  Date: 29/08/2018
