# ML-HomeWork-4

# Sai Sahith Pasumarthy #700769267

# Question 2: NLP: Named Entity Recognition & Pronoun Ambiguity Detection

This project performs **Named Entity Recognition (NER)** and detects potential **pronoun ambiguity** in a given text.

It uses:

-  spaCy automatically **if installed**
-  A **fallback rule-based NER** if spaCy isn't available  
  *(ensures the script runs even in restricted environments such as some Google Colab runtimes)*

---

##  Features

| Feature | Description |
|--------|-------------|
| Named Entity Recognition | Detects names of people, companies, places, products |
| Pronoun Ambiguity Warning | Prints a warning if text contains pronouns like *he/she/they* |
| Model Fallback | Falls back to rule-based NER when no NLP model is available |
| Fully Portable | Runs in most Python environments without failing installations |

---

##  Example Input: Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch.
Warning: Possible pronoun ambiguity detected!
Entities: [('Chris', 'PERSON'), ('Alex', 'PERSON'), ('Apple', 'ORG'), ('California', 'GPE'), ('iPhone', 'PRODUCT')]


---

Concepts Used                 Concept	Description
Tokenization	                Breaking text into words
Named Entity Recognition	    Extracting real-world named entities
Coreference Heuristic	        Detecting ambiguous pronouns
Robust NLP	                  Graceful fallback if no model available

---

Academic Context
This project demonstrates:
NER pipeline and entity extraction
Handling pronoun ambiguity 
Practical NLP design for real-world execution environments

---
## Question 1: 
## Question 1: # Minimal NLP Pipeline (No External Libraries)

This project demonstrates a **lightweight NLP preprocessing pipeline** implemented **without any external dependencies**.  
It is designed for environments where installing NLP libraries (spaCy, NLTK) is not possible (e.g., restricted Colab runtimes).

---

##  Features

| Step | Description |
|------|------------|
| Tokenization | Regex-based token extraction |
| Stopword Removal | Removes common English stopwords |
| POS Tagging (Rule-based) | Heuristics to identify NOUN, VERB, PROPN |
| Lemmatization | Hand-crafted rules for verbs & nouns |
| Output | Sequence of cleaned, lemmatized key tokens |

---


How It Works
Component	Method
Tokenization	Regular expressions
Stopwords	Manually defined list
POS Tagging	Simple heuristic rules
Lemmatization	Rule-based verb & noun handling
Output	Final cleaned text with key tokens

Purpose
Understand core NLP preprocessing concepts without libraries
Maintain compatibility with limited execution environments
Demonstrate lemmatization & POS tagging logic manually

No Dependencies
This script does not require:
spaCy
NLTK
NumPy
SciPy
