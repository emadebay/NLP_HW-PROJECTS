run_lr.py Inside NLP_3.zip
This Python script, sentiment_analysis_adjective_features.py, performs sentiment analysis on movie reviews using unique adjectives as features. It utilizes logistic regression to classify movie reviews as positive or negative based on the adjectives present in the text. Below is an overview of the functionalities provided by each section of the script:

Setup: This section imports necessary libraries and sets up the environment.
Helper Functions: The extract_unique_adjectives function extracts unique adjectives from a text using spaCy. The get_all_the_unique_adjectives function processes all the text files in two folders to obtain a set of unique adjectives. The convert_set_dictionary function maps the unique adjectives to integer indices. The create_a_vector_of_adjective_vocabulary_length function initializes a vector of zeros of a given length. The process_data_into_matrix function converts the processed text data into a matrix format suitable for training the model. The train_and_predict function trains a logistic regression model and predicts sentiment labels for both training and test data.
Training and Testing: This section processes the training and test data, obtains unique adjectives, converts them into matrix format, and trains a logistic regression model. It then evaluates the model's performance using F1 score on both training and test data.
Data Directory Paths: Specifies the directories containing the training and test text files.
Training Data Processing: Processes the training data into matrix format and generates output labels.
Test Data Processing: Processes the test data into matrix format.
Model Training and Evaluation: Trains the logistic regression model and evaluates its performance on training and test data.
To use this script, make sure to have the necessary text files organized in the specified directory structure. Execute the script in a Python environment, and it will perform sentiment analysis on the movie reviews using adjective features, providing insights into the model's performance on both training and test data.

hw4_nlp.py
NLP Homework 4: Fine-Tuning DistilBERT for Sentiment Analysis
This notebook contains the code for fine-tuning the DistilBERT model for sentiment analysis on the IMDb movie review dataset. The notebook is organized into several sections, each corresponding to a specific task in the homework assignment.

Contents:
Introduction
Brief overview of the notebook's purpose and organization.
Data Loading and Preprocessing (Question A)
Reading in the train and test data.
Splitting the data into positive and negative examples.
Creating Validation Sets (Question B)
Splitting the training data into train and validation sets.
Tokenization with DistilBERT (Question C)
Tokenizing the texts using the DistilBERT tokenizer.
Dataset Creation for PyTorch (Question D)
Creating PyTorch Dataset objects from tokenized inputs.
Model Training (Questions E and F)
Fine-tuning the DistilBERT model for sentiment analysis.
Training the model and evaluating on the validation set.
Model Evaluation (Question F)
Evaluating the trained model on the test dataset.
Calculating classification metrics such as accuracy, precision, recall, and F1-score.
Usage:
To run the notebook:

Set up the environment:
Make sure to have access to a GPU if available for faster training.
Install the required libraries (transformers, torch) if not already installed.
Upload the IMDb movie review dataset:
Ensure that the train and test data directories are correctly specified.
The data should be organized into positive and negative examples within each set.
Execute each cell in the notebook sequentially:
Run each cell to load the data, tokenize it, create datasets, train the model, and evaluate its performance.
Review the results:
Examine the classification metrics printed at the end of the notebook to assess the model's performance.
Optionally, explore further by analyzing incorrect predictions, fine-tuning hyperparameters, or experimenting with different model architectures.
Requirements:
Python 3
PyTorch
Hugging Face Transformers
