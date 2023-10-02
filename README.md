# Language_translation
  
This code sets up a Transformer-based sequence-to-sequence model for Spanish-English translation. I

##DATA PREPROCESSING-

Preprocesses the data by splitting it into English and Spanish pairs and adding special tokens [start] and [end] to indicate the start and end of a sentence.

##Data Shuffling and Splitting:

Shuffles the dataset and splits it into training, validation, and test sets.


**Vocabulary and Text Vectorization:
**
Sets up text vectorization layers for English and Spanish texts.
Standardizes the text by converting it to lowercase and removing punctuation.


**Dataset Formatting:
**
Defines functions to format the dataset, converting text to integer sequences.
Slices the target sequences for decoder input and output.


**Dataset Creation and Batching:
**
Creates TensorFlow datasets for training and validation, batching them.


**Model Definition:
**
Defines the Transformer Encoder, Positional Embedding, and Transformer Decoder as explained in your previous message.


**Model Instantiation:
**
Instantiates the encoder and decoder models and establishes the connections between them.


**Model Compilation:
**
Compiles the full Transformer model using RMSprop optimizer and sparse categorical cross-entropy loss.


**Model Training:
**
Trains the model on the training dataset for one epoch (you might want to increase this for better convergence).
Provides validation data.


**Model Summary:
**
Prints out a summary of the model architecture.


**Training Results:
**
After training, the model's performance metrics (loss and accuracy) on both training and validation sets are displayed.



This code contains three classes - TransformerEncoder, PositionalEmbedding, and TransformerDecoder. which work togeather to form a transformer-based neural network model.

TransformerEncoder: This class represents a Transformer encoder layer. It includes multi-head attention, dense projections, and layer normalization operations. It is responsible for encoding input data.

PositionalEmbedding: This class handles the positional embeddings of the input tokens. It combines token embeddings and positional embeddings and is used to inject information about the position of tokens into the model.

TransformerDecoder: This class represents a Transformer decoder layer. It also includes multi-head attention, dense projections, and layer normalization operations. It takes both the input and the output of the encoder as inputs, and it is responsible for generating output sequences.


