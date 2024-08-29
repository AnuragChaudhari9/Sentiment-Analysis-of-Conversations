# Bussiness Meeting Dialogue Analysis
## Overview
This project analyses dialogues between an agent and a customer, discussing life insurance options in this example. The code processes text files containing dialogue, categorizes the dialogue based on sentiment, and extracts key topics from positive and concern-related statements for both the agent and the customer.

## Key Features
__Sentiment Analysis:__ Uses a pre-trained DistilBERT model fine-tuned for sentiment analysis to classify each sentence in the dialogue as positive, neutral, or negative (concern).<br>
__Topic Extraction:__ Extracts key topics from the dialogue by identifying the most representative sentences within each sentiment category.<br>
__Dialogue Parsing:__ Handles the parsing of text files where dialogue is structured with speakers identified by names followed by a colon (:).<br>

## Dependencies
This project relies on the following Python libraries:

__nltk:__ Used for sentence tokenization.<br>
__transformers:__ Provides pre-trained models for sentiment analysis and embedding generation.<br>
__torch:__ Required for running models from the transformers library.<br>
__numpy:__ Used for numerical operations, including computing cosine similarity.<br>
__scikit-learn:__ Used for calculating cosine similarity between sentence embeddings.<br>

## Output
The script categorizes and extracts topics based on the dialogue sentiment:

__Agent's Positive Topics:__ Sentences that reflect positive information or sentiment provided by the agent.<br>
__Agent's Concern Topics:__ Sentences that indicate potential concerns or issues addressed by the agent.<br>
__Customer's Positive Topics:__ Sentences reflecting the customer's positive reactions or appreciation.<br>
__Customer's Concern Topics:__ Sentences where the customer expresses concerns or asks about potential issues.<br>

## File Structure
__life_insurance_conversation.txt:__ Example input file containing the dialogue.<br>
__dialogue_analysis.py:__ Main Python script containing the code for dialogue analysis.<br>
