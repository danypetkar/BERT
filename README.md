# Understanding BERT Model
BERT, which stands for Bidirectional Encoder Representations from Transformers, is based on transformers, a deep learning model in which every output element is connected to every input element and the weightings between them are dynamically calculated based upon their connection.

Historically, language models could only read input text sequentially either left-to-right or right-to-left but couldn’t do both at the same time.

BERT is different because it’s designed to read in both direction at once. The introduction of transformer models enabled this capability, which is known as bidirectionality.

One of the latest milestones in this development is the release of BERT, an event described as marking the beginning of a new era in NLP. BERT is a model that broke several records for how well models can handle language-based tasks.

BERT builds on top of a number of clever ideas that have been bubbling up in the NLP community recently – including but not limited to Semi-Supervised Sequence Learning, ELMo, ULMFiT, OpenAI transformer, and the Transformer.
## Model Architecture
Two model sizes for BERT:

•	BERT BASE – Comparable in size to the OpenAI Transformer in order to compare performance.

•	BERT LARGE – A ridiculously huge model which achieved the state of the art results.

#### BERT is basically a trained Transformer Encoder stack.


## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

## Model Inputs
![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

The first input token is supplied with a special [CLS] token for reasons that will become apparent later on. CLS here stands for Classification.

Just like the encoder of the transformer, BERT takes a sequence of words as input which keep flowing up the stack. Each layer applies self-attention, and passes its results through a feed-forward network, and then hands it off to the next encoder.
## Model Outputs
Each position outputs a vector of size hidden_size (768 in BERT Base). For the sentence classification example we’ve looked at above, we focus on the output of only the first position (that we passed the special [CLS] token to).

That vector can now be used as the input for a classifier of our choosing. The paper achieves great results by just using a single-layer neural network as the classifier.

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

#### Using bidirectionally, BERT is pretrained on two different but related NLP tasks: Masked language modelling (MLM) and next sentence prediction (NSP)
## Masked Language Model (MLM):
The objective of MLM training is to hide a word in a sentence and then have the program predict what word has been hidden based on the hidden word’s context.
## Next Sentence Prediction (NSP):
NSP is a training technique that teaches BERT to predict whether a certain sentence follows a previous sentence to test its knowledge of relationships between sentences. 
## Applications
    1.	Text Classification
    2.	Text Summarization
    3.	Language Modeling & Text Generation
    4.	Text Similarity and Paraphrasing
    5.	Sentiment and Emotion Detection in Chatbots
    6.	Question Answering (QA)
    7.	Named Entity Recognition (NER)
    8.	Legal and Healthcare Document Analysis






