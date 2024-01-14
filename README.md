# NLP Assignment 2 Case 2


# Hierarchical Document Summarization

## Overview

This project implements a hierarchical document summarization pipeline. The method is developed as part of the NLP course for a Master's degree in Artificial Intelligence at the University of Verona. It is based on providing a set of N documents. The goal is to generate summaries for each document, collate these summaries based on a specified number of steps, and recursively generate the summary of the summaries until the number of steps is exhausted.

## Features

- **Document Generation**: Generates a set of fake documents with a specified number of paragraphs.
- **Word Frequency Table**: Creates a word frequency table from the given text, excluding stop words.
- **Tokenization and Scoring**: Tokenizes text into sentences, scores each sentence based on term frequency.
- **Threshold Calculation**: Finds the threshold by calculating the average score of sentences.
- **Summary Generation**: Generates a summary by selecting sentences with scores above the threshold.
- **Collation**: Collates document summaries based on the specified number of steps.
- **Hierarchical Summarization**: Implements hierarchical summarization according to the specified steps.
- **Total Token Calculation**: Prints the total tokens for all generated documents.
- **Context Window Handling**: Checks if the total tokens exceed the context window size and summarizes accordingly.

## Requirements

- Python 3.x
- Required Python packages (install using `pip install -r requirements.txt`):
  - nltk
  - faker

## Configuration

Adjust the following parameters in the script according to your needs:

- `num_fake_documents`: Number of fake documents to generate.
- `paragraphs_per_document`: Number of paragraphs in each fake document.
- `steps`: Number of steps for hierarchical summarization.
- `max_tokens`: Maximum allowed tokens in the context window.

## File Output

- Fake documents are saved in files named `fake_document_{i}.txt`.
- Summaries are saved in files named `summary_{i}.txt`.
- Summary of summaries is saved in the file `summary_of_summaries.txt`.

## License

This project is licensed under the MIT License.


