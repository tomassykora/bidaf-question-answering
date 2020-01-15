# bidaf-question-answering

A Bi-Directional Attention Flow (BiDAF) question answering model enhanced by 2 convolutional network layers with batch normalisation and a residual connection for the character embeddings as the input to the bidirectional LSTM layer.

Proposed improvements of 4.94 and 5.11 percentage points in EM and F1 scores respectively are described in the [paper](https://github.com/tomassykora/bidaf-question-answering/blob/master/paper.pdf) (although there was only one experiment with the batch norm. layer which means many improvements ahead!).

Character embedding layers | EM | F1 |
--- | --- | --- |
1-layer cnn emb | 58.23 | 61.44
2-layer cnn emb + residual | 59.57 | 62.90 
2-layer cnn emb + residual | 60.46 | 63.65 
2-layer cnn emb + residual + batch norm. | 63.17 | 66.55 

This project is originally from [CS224n](http://web.stanford.edu/class/cs224n/) (winter 2020), but solved for Brno University of Technology, Faculty of Information Technologies, course [ZPJa](https://www.fit.vut.cz/study/course/13531/) - Natural Language Processing.

Based on the paper - [Bidirectional Attention Flow for Machine Comprehension](https://arxiv.org/abs/1611.01603) (2018).
