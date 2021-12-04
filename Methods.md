# **Natural language processing**  

<u>**Step 1:**</u> Tokenization - performed using the TensorFlow is a Python library that invokes C++ to
construct and execute dataflow graphs. It supports many classification and regression algorithms,
and more generally, deep learning and neural networks. Furthermore, fit_on_texts method was
used so that the tokenizer goes through all the tokens or words and fits itself to most frequent
used.  

<u>**Step 2:**</u> Turning sentences into data i.e we tried forming sequences for a given sentence using the
text_to_sequences method this method converts the tokens to a given sentence sequence also all
the sentences are set to length of the longest sequence using the pad_sequences method we also
specified certain parameters (sequences, padding,maxlen) while using this function so that we
can specify the maximum length of the padded sequences. Furthermore,if sentences are longer
than the specified maxlen the sentence was truncated (we can either post or pre truncate) using
the parameter truncating in the pad_sequences method.  

<u>**Step 3:**</u> Training a model to recognize sentiment in text - we started training the model after
completing the pre-processing step,a classifier was built to recognize the sentiments in a given
text.We used the dataset of news headlines, where the headlines have been classified into two
categories sarcastic or not.  

<u>**Step 4:**</u> Creation of set of training and test sequences for training and test sets under the name of
training_sequences and testing_sequences respectively
The words can be categorized as good or bad, but words like not bad means something which is
not equal to good, probably lesser than good and but not necessarily bad. Therefore, we consider
words having sentiment as vectors and plot them in various dimensions to measure if they are
bad, good, sad, happy, etc.Words that appear only in the sarcastic sentences, their vectors would
be a bit more towards the sarcastic direction than the unsarcastic direction. Therefore, training
the model with such a vector will enhance the accuracy of the model. We will feed the fully
trained model with test data, the model will look up to the trained vectors and sum up each
word's vector for a final direction. This will tell us if the sentence was sarcastic or not. This
concept is called Embedding.  

<u>**Step 5:**</u> Training the neural network model for the same- this was performed using the tensorflow
library, for this specific model we deployed Adam's optimizer and accuracy as the metric for
evaluating the model’s accuracy.  

<u>**Step 6:**</u> Visualization of the results - using the matplotlib library we were able to plot the graph of
accuracy v/s epochs so that we can analyze the model’s accuracy.  

<u>**Step 7:**</u> Predicting the class label for the test set- Here, the first sentence was predicted to be
sarcastic with a probability of 0.9999 (approx 1) whereas for the second sentence it had the
probability of 0.0007 ( approx 0). This clearly means that the first sentence is very close to being
sarcastic and the second sentence is not at all close to being sarcastic.
