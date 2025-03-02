# Extractive Text Summarization

This project implements an extractive text summarization approach that assigns importance scores to sentences based on multiple factors. The method ensures that the most relevant sentences are retained while generating concise and meaningful summaries.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## Introduction
Text summarization is an essential task in natural language processing (NLP) that helps extract key information from large text documents. This project utilizes a weighted sentence approach where sentences are scored based on word frequency, length, numerical data presence, and similarity to the title. By leveraging these factors, the model effectively generates structured summaries while preserving the core meaning of the text.

## Features
- **Word Frequency Analysis**: Prioritizes sentences with high-frequency words to reflect overall document importance.
- **Sentence Length Consideration**: Weights longer sentences higher, assuming they contain more context.
- **Numerical Data Emphasis**: Boosts importance for sentences containing numerical values, which often carry critical insights.
- **Cosine Similarity to Title**: Sentences closely related to the title are ranked higher for contextual relevance.
- **Evaluation Metrics**: Assesses summary quality using BLEU and ROUGE-2 scores.

## Technologies Used
- **Python**: Primary programming language for implementation.
- **SpaCy**: Used for tokenization and NLP tasks.
- **NLTK**: Utilized for sentence tokenization and BLEU score calculation.
- **scikit-learn**: Applied for TF-IDF vectorization and cosine similarity.
- **rouge-score**: Used for ROUGE score evaluation.

## Installation
To set up the project, install the required dependencies using:
```sh
pip install -r requirements.txt
```

## Usage
Run the summarization script by providing an input text file:
```sh
python summarize.py --input document.txt
```
The generated summary will be saved in an output file.

## Evaluation
The quality of the summaries is assessed using:
- **BLEU Score**: Measures precision in n-gram matching between the summary and reference text.
- **ROUGE-2 Score**: Evaluates recall by comparing bigram overlaps with the reference summary.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

## License
This project is open-source under the **MIT License**.

## Author
**Soham Borkar**  
Email: soham.borkar22@vit.edu  
LinkedIn: [Soham Borkar](https://www.linkedin.com/in/soham-borkar-4102342ba/)
