# Building Chatbot Using Python 




## What are chatbots ?

Chatbots/ AI assistants are simulations which can understand human language, process it and interact back with humans while performing tasks assigned to the bot.

## Types of Chatbots

1. Text-based Chatbots
2. Voice-based Chatbots




#### **Chatbots are designed using 2 approaches:**

* **Rule-based Chatbot** : Bot answers to the questions based on some rules on which it is trained on. 
* **Self-learning Chatbot** : Bot learns how to communicate based on a 'Machine learning model' to learn and asess current situation.


## About Project

In this Project, we've prepared a chatbot that learns from a corpus using *Natural Language Processing*(NLP) techniques.


 **Tools & technologies:**

* Libraries used : nltk, string, random
            
#### Import Libraries:

* Natural Language Toolkit(NLTK) : A comprehensive library for NLP in Python.
* String : Provides a collection of string operations.
* Random : Used to generate random choice.

#### Import and Read the corpus:

* Downloads necessary NLTK resources : *Punkt* for sentence tokenization and *wordnet* for lemmatization.
* Tokenizes the text into sentences (sent_tokens) and words (word_tokens).

#### Text Preprocessing :

* Initializes the *WordNet Lemmatizer*. 
* Defines a function *LemTokens* to lemmatize a list of tokens.
* Creates a dictionary to remove punctuation from text.
* Defines a function *LemNormalize* to normalize the text by converting it to lowercase, removing punctuation, and lemmatizing the tokens.

#### Defining greeting functions: 

Defines a list of greeting inputs and responses.

#### Generating Responses:

* Imports necessary modules from *sklearn* for TF-IDF vectorization and cosine similarity.

**scikit-learn** : 

 * *sklearn.feature_extraction.text.TfidfVectorizer*: Converts a collection of raw documents to a matrix of TF-IDF features. **TF-IDF (Term Frequency-Inverse Document Frequency)** is a statistical measure used to evaluate the importance of a word in a document relative to a collection of documents (corpus).

  * *sklearn.metrics.pairwise.cosine_similarity*: Cosine similarity is a measure that calculates the cosine of the angle between two vectors, often used to measure document similarity in text analysis.


#### Chatbot functionalities:

* Greeting Function : "greet(sentence)" Checks if the user's input contains any greeting words and returns a random greeting response.
* Generating responses : "response(user_response)" Generates a response to the user's input using TF-IDF and cosine similarity to find the most relevant sentence from the corpus.

**Conversation Flow** :

* The chatbot continuously takes user input, processes it, and generates responses until the user types 'bye'.
* It handles greetings, thanks, and other conversational inputs, providing appropriate responses or apologizing if it doesn't understand the input.



**These above tools and techniques used to build the Chatbot uses Natutal Language inputs,understand user queries, generate responses based on the text data provided.**



