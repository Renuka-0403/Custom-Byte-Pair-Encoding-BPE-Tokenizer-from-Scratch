# Autoregressive Causal Language Model using Custom Byte-Pair Encoding (BPE)

## Overview

This project implements an **Autoregressive Causal Language Model (ARLM)** from scratch using **Python** and **NumPy**. Before training the language model, a **Custom Byte-Pair Encoding (BPE) Tokenizer** is built from scratch to learn subword tokens from a text corpus. The learned BPE tokenizer converts text into token IDs, which are then used as input for the autoregressive language model.

The project demonstrates the complete workflow of text tokenization, embeddings, positional encoding, causal self-attention, next-token prediction, and text generation.

---

## Objectives

- Implement a Custom Byte-Pair Encoding (BPE) Tokenizer from scratch.
- Learn subword vocabulary by repeatedly merging the most frequent symbol pairs.
- Encode and decode text using learned merge rules.
- Build an Autoregressive Causal Language Model.
- Predict the next token using only previously seen tokens.
- Demonstrate text generation using the trained model.

---

## Features

- Custom BPE Tokenizer
- Corpus preprocessing
- Character-level tokenization
- Pair frequency counting
- Merge rule learning
- Encode and Decode functions
- Token ID generation
- Input–Target pair creation
- Embedding layer
- Positional Encoding
- Causal Self-Attention
- Linear Output Layer
- Softmax activation
- Cross-Entropy Loss
- Simple training loop
- Interactive next-token prediction
- Text generation

---

## Project Structure

```
Autoregression_Model.ipynb
corpus.txt
README.md
```

---

## Input Corpus

Example (`corpus.txt`)

```
low
lower
lowest
new
newer
widest
```

---

## BPE Algorithm Flow

```
Start
   ↓
Read Text Corpus
   ↓
Preprocess Text
   ↓
Split Words into Characters + </w>
   ↓
Count Word Frequencies
   ↓
Find Adjacent Symbol Pairs
   ↓
Count Pair Frequencies
   ↓
Select Most Frequent Pair
   ↓
Merge Pair
   ↓
Update Vocabulary
   ↓
Repeat Until Vocabulary Size Reached
   ↓
Store Merge Rules
   ↓
Build Final Vocabulary
   ↓
Encode & Decode
   ↓
End
```

---

## Autoregressive Language Model Pipeline

```
Raw Text
      ↓
Byte Pair Encoding (BPE)
      ↓
Token IDs
      ↓
Input–Target Pairs
      ↓
Embedding Layer
      ↓
Positional Encoding
      ↓
Causal Self-Attention
      ↓
Linear Layer
      ↓
Softmax
      ↓
Cross-Entropy Loss
      ↓
Next Token Prediction
      ↓
Text Generation
```

---

## Sample Output

### Example 1

```
============================================================
TEXT GENERATION
============================================================

Enter a word : low

Input : low
Encoded : ['low</w>']

Predicted Next Token : er

Generated Word : lower
```

### Example 2

```
============================================================
TEXT GENERATION
============================================================

Enter a word : new

Input : new
Encoded : ['new</w>']

Predicted Next Token : er

Generated Word : newer
```

---

## Technologies Used

- Python
- NumPy
- Jupyter Notebook

---

## Learning Outcomes

Through this project, the following concepts were implemented and understood:

- Byte-Pair Encoding (BPE)
- Subword Tokenization
- Vocabulary Learning
- Token IDs
- Word Embeddings
- Positional Encoding
- Query, Key and Value Matrices
- Causal Self-Attention
- Softmax
- Cross-Entropy Loss
- Next Token Prediction
- Autoregressive Text Generation

---

## Conclusion

This project successfully implements a **Custom Byte-Pair Encoding (BPE) Tokenizer** and an **Autoregressive Causal Language Model** from scratch using Python and NumPy. The BPE tokenizer learns subword vocabulary through iterative merge operations and converts text into token IDs. These token IDs are then processed by the autoregressive language model using embeddings, positional encoding, causal self-attention, and a linear output layer to predict the next token. The interactive text generation feature demonstrates how previous context can be used to generate subsequent tokens, providing a practical understanding of the core principles behind modern Transformer-based language models.

---
