# 🧩 Custom Byte-Pair Encoding (BPE) Tokenizer from Scratch

A Python implementation of the **Byte-Pair Encoding (BPE) Tokenizer** from scratch without using any tokenizer libraries or pretrained models. This project demonstrates how BPE learns subword vocabularies through iterative pair merging and uses the learned merge rules to encode and decode words.

---

## 📌 Project Overview

Byte-Pair Encoding (BPE) is a subword tokenization algorithm widely used in modern Natural Language Processing (NLP) models such as GPT, BERT, RoBERTa, and T5. It reduces the vocabulary size by merging the most frequent adjacent symbol pairs, enabling efficient handling of rare and unseen words.

This project implements the complete BPE tokenizer pipeline from scratch using Python.

---

## 🎯 Objectives

- Implement the Byte-Pair Encoding algorithm from scratch.
- Learn subword vocabulary from a text corpus.
- Generate merge rules based on pair frequencies.
- Build the final vocabulary.
- Encode new words using the learned merge rules.
- Decode encoded tokens back into the original words.

---

## ✨ Features

- Read text corpus from a file
- Text preprocessing
- Character-level vocabulary creation
- Word frequency counting
- Adjacent pair frequency calculation
- Iterative pair merging
- Learned merge rule generation
- Final vocabulary creation
- Encode new words into subword tokens
- Decode tokens back into words

---

## 🛠️ Technologies Used

- Python 3
- NumPy
- Jupyter Notebook

---

---

## ⚙️ Algorithm Workflow

```
Text Corpus
      │
      ▼
Read Corpus
      │
      ▼
Preprocess Text
      │
      ▼
Split Words into Characters
      │
      ▼
Append </w>
      │
      ▼
Count Word Frequencies
      │
      ▼
Find Adjacent Symbol Pairs
      │
      ▼
Count Pair Frequencies
      │
      ▼
Select Most Frequent Pair
      │
      ▼
Merge Pair
      │
      ▼
Update Vocabulary
      │
      ▼
Repeat for N Merges
      │
      ▼
Store Merge Rules
      │
      ▼
Build Final Vocabulary
      │
      ▼
Encode New Words
      │
      ▼
Decode Tokens
```

---

## 📖 Implementation Steps

1. Read the text corpus.
2. Preprocess the input text.
3. Split words into characters.
4. Append the end-of-word symbol (`</w>`).
5. Count word frequencies.
6. Find adjacent symbol pairs.
7. Calculate pair frequencies.
8. Select the most frequent pair.
9. Merge the selected pair.
10. Update the vocabulary.
11. Repeat the merge process.
12. Store merge rules.
13. Build the final vocabulary.
14. Encode new words.
15. Decode encoded tokens.

---

## 📊 Sample Output

The notebook displays:

- Initial Vocabulary
- Word Frequencies
- Pair Frequencies
- Merge Operations
- Updated Vocabulary
- Final Vocabulary
- Learned Merge Rules
- Encoded Words
- Decoded Words

## 📚 Key Concepts Covered

- Byte-Pair Encoding (BPE)
- Subword Tokenization
- Vocabulary Learning
- Pair Frequency Analysis
- Merge Rules
- Encoding
- Decoding
- Natural Language Processing (NLP)
- Python Programming

---

## 🎓 Learning Outcomes

Through this project, I learned:

- The working principles of Byte-Pair Encoding.
- How subword vocabularies are generated.
- Frequency-based pair merging.
- Tokenization using learned merge rules.
- Manual implementation of NLP algorithms.
- The role of BPE in Transformer-based language models.

---


## 📝 Conclusion

This project demonstrates the implementation of a **Custom Byte-Pair Encoding (BPE) Tokenizer** from scratch using Python and NumPy. It covers the complete workflow of learning subword vocabularies through iterative pair merging and applying the learned merge rules to encode and decode words. This implementation provides a strong foundation for understanding subword tokenization techniques used in modern Transformer-based NLP models.

---
