# Transformers Pipeline Functions for NLP Tasks

This repository demonstrates the usage of Hugging Face's Transformers pipeline functions for various Natural Language Processing (NLP) tasks. The project showcases how to use different pre-trained models to perform common NLP tasks using the pipeline API.

## Features

The project demonstrates the following NLP tasks using Transformers pipeline:

1. **Sentiment Analysis**
   - Analyzes restaurant reviews to determine positive/negative sentiment
   - Uses DistilBERT model for sentiment classification
   - Visualizes sentiment distribution

2. **Zero-Shot Classification**
   - Classifies text into predefined categories without training
   - Demonstrates classification of text into education, politics, and business categories
   - Shows confidence scores for each category

3. **Text Generation**
   - Generates new text based on input prompts
   - Uses GPT-2 model for text generation
   - Demonstrates creative text completion

4. **Named Entity Recognition (NER)**
   - Identifies and classifies named entities in text
   - Uses BERT model for entity recognition
   - Groups related entities together

5. **Fill-Mask**
   - Predicts missing words in text
   - Uses DistilRoBERTa model
   - Shows top-k predictions for masked tokens

6. **Question Answering**
   - Answers questions based on given context
   - Uses DistilBERT model
   - Demonstrates extractive question answering

7. **Text Summarization**
   - Generates concise summaries of input text
   - Uses DistilBART model
   - Creates abstractive summaries

8. **Translation**
   - Translates text between languages
   - Uses Helsinki-NLP models
   - Demonstrates English to Romance language translation

## Requirements

- Python 3.x
- transformers
- pandas
- matplotlib
- torch

## Installation

```bash
pip install transformers pandas matplotlib torch
```

## Usage

The notebook demonstrates how to use each pipeline function with example code and explanations. Each section includes:
- Model initialization
- Example input
- Output demonstration
- Explanation of results

## Example

```python
from transformers import pipeline

# Sentiment Analysis
sentiment_analyzer = pipeline("sentiment-analysis")
result = sentiment_analyzer("I love this restaurant!")
print(result)

# Zero-Shot Classification
classifier = pipeline("zero-shot-classification")
result = classifier(
    "This is a text about technology",
    candidate_labels=["technology", "sports", "politics"]
)
print(result)
```

## Models Used

- DistilBERT
- GPT-2
- BERT
- DistilRoBERTa
- DistilBART
- Helsinki-NLP models

## Contributing

Feel free to submit issues and enhancement requests!

## Contact

- Email: ypssefmohammedahmed@gmail.com
- Phone: +20 1126078938

## License

This project is licensed under the MIT License - see the LICENSE file for details.
