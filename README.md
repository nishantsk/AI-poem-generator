# AI-poem-generator
It's a AI model generating poems by it self

# Installation
In order to get the poetry generator to run, you need Python 3. Here we have used google colab for our project.
We have done the most of the work in tensorflow library 

# Model Building
For computer to understand the words, firstly we had to tokenize the whole dataset using tokenizer after loading the dataset.
Then we splitted the dataset into two for training and testing purposes. We have applied the n-gram technique on the dataset.
Here we have taken individual tokenized line from starting and created the n-grams in order to predict the next word. consider a tokenized line and using n-grams method we have created lists from the tokenized line like first two , first three and so on. The reason behind this is that we want to predict the next  word after the first two , first three words and so on , by training the model on this algorithm , the machine can predict the next word when it will see these two words together or these three words together and similarly. In order to put the list of input sequences in the same dimension we have padded the lists according to the line of maximum length in the dataset. Using neural networks
we have set epochs = 30 and because of this it will propagate back and forth in the layer 30 times to increase the accuracy.

# Training model 
Using the above algorithm we have trained our data on the training datset.

# Generating the poem
Now using the test dataset we are creating the AI generated poem and it came out in the form of a paragraph and now the problem is that we got it in the form of paragraph and a sonnet is a poem of 14 line and then using the code we have converted it into the 14 line poem


