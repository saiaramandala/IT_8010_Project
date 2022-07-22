<div id="top"></div>




<!-- PROJECT SHIELDS -->




<h3 align="center">Fake News Classification with Keras</h3>


<!-- ABOUT THE PROJECT -->
## About The Project

This project looks at building, training and evaluating neural networks to solve the [fake news classification problem](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset) on Kaggle. It uses Python and Keras. 

Gated Recurrent Units (GRUs) are used, along with batch normalization and both spaCy and Keras embedding layers. 

Keras embedded models appear to outperform those with a static spaCy embedding and manage to achieve extremely high test accuracies (99%+).

The run_models.ipynb notebook contains a demo of how code from the two Python files can be used to easily implement the networks needed to solve this task.

## About The Data

The data for this task is taken from a Kaggle dataset of around 45K news articles. Around half of the data are fake articles pulled from various US-based websites that have been deemed unreliable by fact-checking organisations, with the other half being true articles pulled from Reuters, a US news website.

An example of what these articles look like can be seen below.

<img width="1440" alt="Screen Shot 2022-07-19 at 2 42 22 PM" src="https://user-images.githubusercontent.com/30325044/179825780-48d1c50b-d80a-4f5b-bcd4-1af7d55cd906.png">

Given that all of the articles are coming from US sources and that all of the true articles are coming from the same US source, this is clearly not a perfect fake news dataset. Others have also identified some leakage in the dataset. Leakage is when information is available in the training data for a model to predict with that it wouldn’t have access to in the real world. Steps will be taken in the pre-processing to try and minimise the impacts of this leakage.



### Neural Networks

A neural network is a network or circuit of biological neurons, or, in a modern sense, an artificial neural network, composed of artificial neurons or nodes. Thus, a neural network is either a biological neural network, made up of biological neurons, or an artificial neural network, used for solving artificial intelligence (AI) problems. The connections of the biological neuron are modeled in artificial neural networks as weights between nodes. A positive weight reflects an excitatory connection, while negative values mean inhibitory connections. All inputs are modified by a weight and summed. This activity is referred to as a linear combination. Finally, an activation function controls the amplitude of the output. For example, an acceptable range of output is usually between 0 and 1, or it could be −1 and 1.

### Gated Recurrent Units (GRUs)

Gated recurrent units (GRUs) are a gating mechanism in recurrent neural networks, introduced in 2014 by Kyunghyun Cho et al. The GRU is like a long short-term memory (LSTM) with a forget gate, but has fewer parameters than LSTM, as it lacks an output gate. GRU's performance on certain tasks of polyphonic music modeling, speech signal modeling and natural language processing was found to be similar to that of LSTM. GRUs have been shown to exhibit better performance on certain smaller and less frequent datasets.

### SpaCy

spaCy is an open-source software library for advanced natural language processing, written in the programming languages Python and Cython. The library is published under the MIT license and its main developers are Matthew Honnibal and Ines Montani, the founders of the software company Explosion. Unlike NLTK, which is widely used for teaching and research, spaCy focuses on providing software for production usage. spaCy also supports deep learning workflows that allow connecting statistical models trained by popular machine learning libraries like TensorFlow, PyTorch or MXNet through its own machine learning library Thinc. Using Thinc as its backend, spaCy features convolutional neural network models for part-of-speech tagging, dependency parsing, text categorization and named entity recognition (NER). Prebuilt statistical neural network models to perform these tasks are available for 17 languages, including English, Portuguese, Spanish, Russian and Chinese, and there is also a multi-language NER model. Additional support for tokenization for more than 65 languages allows users to train custom models on their own datasets as well.

### Tensorflow

TensorFlow is a free and open-source software library for machine learning and artificial intelligence. It can be used across a range of tasks but has a particular focus on training and inference of deep neural networks. TensorFlow was developed by the Google Brain team for internal Google use in research and production. The initial version was released under the Apache License 2.0 in 2015. Google released the updated version of TensorFlow, named TensorFlow 2.0, in September 2019. TensorFlow can be used in a wide variety of programming languages, most notably Python, as well as Javascript, C++, and Java. This flexibility lends itself to a range of applications in many different sectors.

<p align="right">(<a href="#top">back to top</a>)</p>

### GRU Spacy Embedding

<img width="1067" alt="Spacy Embedding" src="https://user-images.githubusercontent.com/30325044/180579501-ffa8b159-0a7f-436a-82c5-6fa759c8801d.png">

### GRU Keras Embedding

<img width="944" alt="Keras Embedding" src="https://user-images.githubusercontent.com/30325044/180579546-3fbff3ec-87af-44cd-8951-948e5c87b9b6.png">

### Keras vs SpaCy Accuracy Scores

<img width="1083" alt="Keras Vs Spacy Accuracy scores" src="https://user-images.githubusercontent.com/30325044/180579614-02529f53-5c06-4c58-9d50-69f1ca6eb5ae.png">


### Built With

* [Keras](https://keras.io/)
* [spaCy](https://spacy.io/)
* [Tensorflow](https://www.tensorflow.org/)

<p align="right">(<a href="#top">back to top</a>)</p>





<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [othneildrew - README template](https://github.com/othneildrew/Best-README-Template/blob/master/BLANK_README.md)
* [Fake News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
* [Information Leaks in Kaggle Fake News Dataset](https://www.kaggle.com/code/mosewintner/5-data-leaks-100-acc-1-word-99-6-acc?scriptVersionId=45283074)
* Ahmed H, Traore I, Saad S. “Detecting opinion spams and fake news using text classification”, Journal of Security and Privacy, Volume 1, Issue 1, Wiley, January/February 2018.
* Ahmed H, Traore I, Saad S. (2017) “Detection of Online Fake News Using N-Gram Analysis and Machine Learning Techniques. In: Traore I., Woungang I., Awad A. (eds) Intelligent, Secure, and Dependable Systems in Distributed and Cloud Environments. ISDDC 2017. Lecture Notes in Computer Science, vol 10618. Springer, Cham (pp. 127-138).

<p align="right">(<a href="#top">back to top</a>)</p>


