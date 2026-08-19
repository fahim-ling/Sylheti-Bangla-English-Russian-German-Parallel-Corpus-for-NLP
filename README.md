# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)
![Domain: NLP / Computational Linguistics](https://img.shields.io/badge/Domain-NLP%20%2F%20CL-blue)

Welcome to the first open-source multilingual parallel corpus for the **Sylheti** language, designed to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and **Large Language Model (LLM) training**.

> ⚠️ **NOTICE: FULL DATASET IS ON HUGGING FACE (GATED ACCESS)**
> To protect the dataset from unauthorized scraping and AI degradation, the full production datasets are hosted exclusively on Hugging Face. **[Access the Full Dataset Here (Hugging Face) ➔]((https://huggingface.co/datasets/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP))**

## 📂 Sample Dataset Structure
This GitHub repository contains **Sample Data** (50 rows each) to allow researchers and developers to test their Python scripts, tokenizers, and NLP pipelines without needing immediate access to the full gated corpus.

* **Format:** TSV (Tab-Separated Values) / UTF-8 Encoded
* **Sample Files in this Repo (`data/`):** 
  * `sample_parallel_sentences.tsv`: 50 sample parallel sentences across 5 languages.
  * `sample_lexicon.tsv`: 50 sample words and core vocabulary entries.

## 📥 Usage & Data Loading
Since the dataset uses strict Tab-Separated Values (TSV) to accommodate complex scripts (like Syloti Nagri), always use the `\t` separator and UTF-8 encoding when loading the data in Python:

```python
import pandas as pd

# Load the sample lexicon or parallel sentences
df = pd.read_csv('data/sample_parallel_sentences.tsv', sep='\t', encoding='utf-8')
print(df.head())
```
