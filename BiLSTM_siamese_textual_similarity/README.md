# Text Similarity Using Siamese LSTM Deep Neural Network
Siamese neural network is a class of neural network architectures that contain two or more identical subnetworks. identical here means they have the same configuration with the same parameters and weights. Parameter updating is mirrored across both subnetworks.
It is a keras based implementation of deep siamese Bidirectional LSTM network to capture phrase/sentence similarity using word embeddings.

## What's in this repo?

* Code containing the configuration details such as dropout rate, number of LSTM layers, activation function etc., in config.py
* Code containing the embedding technique in controller.py
* Code containing the preprocessing of input data in inputHandler.py
* Code containing the model details in model.py

Datasets are present in \Dataset

Install dependencies
pip install -r requirements.txt
References:
Siamese Recurrent Architectures for Learning Sentence Similarity (2016).
Inspired from Tensorflow Implementation of https://github.com/amansrivastava17/lstm-siamese-text-similarity and https://github.com/dhwajraj/deep-siamese-text-similarity."# NLP" 
