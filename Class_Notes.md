# Natural Language Processing
## Introduction
* What is NLP?

* Why study NLP?
  It must be important, It must be interesting
  Importance : Impact and/or potential impact on our everyday life
  Interesting : New insight, fresh challenge
  
* Why NLP is important?
  Teach computers to communicate with people:
  Database query interfaces ,
  Intelligent tutoring systems,
  Question-answering systems,
  Speech recognition and spoken language understanding

  Help people communicate with each other:
  Machine translation,
  Natural language Generation

  Harness the potential of web:
  Information extraction
  Search (related taskws: classify , filter, summarixe)
  
* NLP has two parts:
* Natural language Understanding(NLU): In which I/P is natural language text and O/P is representation of meaning of text
* Natural language Generation(NLG): In which I/P is non-textual representation like Graph, a time series data and O/P is natural language text.
* NLP = NLU + NLG
* Understanding ---> flight Landing(needs piloting)
* Generation ---> Flight Take-off(can be automated)
* 
### Why NLP is Hard?

### Why NLP is useful?

### Classical Problems

### Speech vs NLP?

## Words
### Structure (Spellcheck, morpholog, and FSTs)
### Semantics
### Part of Speach(Part of Speach Tagging)
#### Classic 
## Sentences
### Compositional Semantics
### Classical Parsing

## Language Modelling


## Machine Translation


## Information Extration


## Deep Learning for NLP



# Extras
## Preprocessing of Documents in NLP
### 1. Text Cleaning
Lowercasing: Converts all text to lowercase to ensure uniformity.
Removing Punctuation and Special Characters: Eliminates unnecessary symbols (e.g., .,!?@#$%).
Removing Stopwords: Filters out common words (e.g., "the," "is," "in") that do not contribute much meaning.
Expanding Contractions: Converts contractions (e.g., "can't" → "cannot").
Correcting Spelling Errors: Uses libraries like TextBlob or SymSpell to fix misspelled words.
Removing Numbers: Eliminates numbers if they are not meaningful for the task.
## 2. Tokenization
Splitting text into individual words (word tokenization) or sentences (sentence tokenization).
Libraries: NLTK, spaCy, Transformers
## 3. Normalization
Lemmatization: Converts words to their base form using vocabulary and morphological analysis (e.g., "running" → "run").
Stemming: Removes word suffixes (e.g., "running" → "runn"), which is less accurate than lemmatization but faster.
## 4. Part-of-Speech (POS) Tagging
Assigns grammatical labels (e.g., noun, verb, adjective) to words.
Useful for contextual analysis.
Libraries: spaCy, NLTK
## 5. Named Entity Recognition (NER)
Identifies entities like names, organizations, dates, and locations in the text.
Libraries: spaCy, Stanford NER
## 6. Removing Noise
Filtering out unnecessary data, such as HTML tags, emojis, and hashtags.
Useful for processing web and social media texts.
## 7. Text Vectorization (Feature Engineering)
Bag of Words (BoW): Converts text into a matrix of word counts.
TF-IDF (Term Frequency-Inverse Document Frequency): Weighs words based on importance.
Word Embeddings (Word2Vec, GloVe, FastText): Captures word meanings based on context.
Transformers (BERT, GPT embeddings): Uses deep learning models to generate contextualized word representations.
## 8. Handling Out-of-Vocabulary (OOV) Words
Replacing rare words with <UNK> or using subword tokenization (Byte Pair Encoding, WordPiece).
## 9. Handling Imbalanced Data (for NLP Classification)
Undersampling or oversampling text data if classes are imbalanced.
## 10. Language Identification and Translation
Detecting language and translating text if necessary.
