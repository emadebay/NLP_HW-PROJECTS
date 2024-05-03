This Python script, HW1.py, is designed to perform several tasks related to text processing and analysis. Below is a brief overview of the functionality provided by each section of the script:

Mounting Google Drive: This script mounts Google Drive to access files stored in Google Drive.
Importing Libraries: The necessary libraries, including matplotlib and nltk, are imported to enable data visualization and text processing.
Class Definition: The HW1 class is defined to encapsulate the methods for performing various text processing tasks.
Setting Input and Output Paths: Two methods, setInputPath and setOutputPath, are provided to set the input file path containing JSON data and the output file path to store extracted messages, respectively.
Reading JSON File and Extracting Messages: The method read_json_file_and_extract_message reads the JSON file, extracts the messages, and stores them in a separate text file.
Splitting Sentences and Tokenization: The method split_using_sent_tokenize_then_use_python_split_to_split_the_sentences_and_nltk_tokenize splits the sentences using nltk.sent_tokenize and tokenizes them using both Python's split method and nltk.word_tokenize.
Counting Tokens and Types: This script counts the number of tokens and types both before and after lowercasing using the split function and nltk tokenization.
Lowercasing All Words: The method lower_case_all_the_words lowercases all words in the text and saves the lowercased content in a new file.
Counting Tokens and Types After Lowercasing: After lowercasing, the script counts the number of tokens and types using nltk tokenization.
Analyzing Word Frequency Distribution: Finally, the script analyzes the word frequency distribution in the text and generates a Zipf's Law graph to visualize the distribution.
To use this script, simply specify the input file path containing JSON data (input_file_path) and the output file path to store extracted messages (output_file_path). Additionally, provide a path to save the lowercased file (lowercased_file_path). Then, execute the script in a Python environment with access to the required libraries.






