# Machine Translation Encoder/Decoder (Character based)

This project demonstrates the concepts on language translation using encoder decoder. This model translate English language to French.

# Dataset Description

Dataset has been taken from the following URL:
http://www.manythings.org/anki/

Data directory: fra_eng/fra.txt

# Keras using Functional API
The functional API is typically used when we want to use multi-input, multi-output models which have many shared layers. Shared layers accept multiple inputs from different sources. 
You can directly initialize the state of shared layers as well.

# Model : The Encoder Decoder for Language Translation

Model has been developed in Keras using Functional API

In order to perform language translation using recurrent neural networks, we use a framework called the encoder-decoder. Encoders are sequence in, vector out RNNs which take in the sequence of words or characters in the input sentence and output a vector which represents the final encoder state. This encoder state encapsulates all the information in the input original sentence. A decoder is an RNN which is a vector in, sequence out RNN. The vector that you feed in is the output of the encoder state. This input vector allows us to predict the sequence, that is the translated sentence at the output. Language translation is clearly a sequence in, sequence out problem which requires an encoder, as well as a decoder. The output of the encoder is fed in as a vector to the decoder. This combination of encoder plus decoder is the recurrent neural network that we'll use for translation. The sequence that we feed in is the characters in the English sentence, and the sequence that we receive at the output is the characters in the French sentence. 

