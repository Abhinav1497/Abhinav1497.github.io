---
layout: page
title: ChatBot using LSTM and CBOW(Continuous Bag of Words)
description: 
img: assets/img/12.jpg
importance: 1
category: work
related_publications: 
---
The purpose of this project is to utilize LSTMs and CBOW to develop a chatbot. More specifically, we will develop a QA bot that aims to answer any question it is given, by leveraging the AmbigQA dataset for training and testing.


Sequence-to-sequence Long Short-Term Memory (LSTM) and Continuous Bag-of-Words (CBOW) are two models that are frequently used in NLP. Long Short-Term Memory (LSTM), which is a type of recurrent neural network (RNN) that is capable of handling long-term dependencies in sequential data, as the name suggests. Unlike RNNs, LSTMs can effectively “remember” and “forget” information over extended periods of time. Compared to standard LSTMs, sequence-to-sequence LSTMs take input sequences and produce sequence outputs as well, rather than fixed values or vectors. As a result, they are effective at capturing contextual information from input data and generating corresponding output predictions, making them ideal for tasks such as speech recognition, natural language processing, and general machine translation.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Code Snippet and Algorithm Flowchart
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


The model takes a sequence of word indices as input, embeds the words into vectors using the embedding layer, processes the embedded sequence using the LSTM layer to capture contextual information, and generates the output prediction using the linear layer. The model learns to generate appropriate responses based on the input sequence by adjusting its parameters during training. See below for a snippet of the ChatBot model:


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Results analysis with epoch loss and accuracy prediction
</div>


Attached above are some screenshots of the results. Firstly, we will discuss the epoch losses. We can see that our overall accuracy ranges from 92% to 93%, which is quite good for a student project, but likely not suitable for any serious applications.
Adjusting the hyperparameters does help, but at the cost of computation time. This is a compromise that has been made for our purposes.
