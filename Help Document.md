Help Document - describes how to execute code and packages used

We used the Google Colab to write code, and execute the code. To execute the code we initially connect to a hosted runtime.
To run the complete code file, goto Runtime -> Run All

---

Google Colab shortcuts

To run a given code cell, press Ctrl+Enter
To convert to markdown/text cells, press Ctrl+M
To convert code cell to markdown/text cell, press Ctrl+M+Y

---

Packages/Library used:

1) Tensorflow library
free and open-source software library for machine learning and artificial intelligence.

2) Keras library from tensorflow
Keras is an open-source software library that provides a Python interface for artificial neural networks. 
Keras acts as an interface for the TensorFlow library. We use Keras library to preprocess the text and form tokens using the Tokenizer class.
We are also using the Pad Sequences class to ensure all sequences have the same dimensions.

3) json package
This package is used to work with the any data that is in json format. This package is included to work with the dataset that is in json format.

4) Numpy library
NumPy, which stands for Numerical Python, is a library consisting of multidimensional array objects and a collection of routines for processing those arrays.
Using NumPy, mathematical and logical operations on arrays can be performed. 
We use NumPy to create arrays for padded sequences for the sentences in the data set.
