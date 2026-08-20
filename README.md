# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License: CC BY-NC 4.0](https://shields.io)
![Domain: NLP / Computational Linguistics](https://shields.io)

Welcome to the **first open-source multilingual parallel corpus** for the **Sylheti (syl)** language, engineered by a native Linguistics student. This dataset bridges Sylheti with four major global high-resource languages spanning **three distinct language families** (Indo-Aryan, Germanic, and Slavic) to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and Large Language Model (LLM) fine-tuning.

> 🚨 **NOTICE: FULL DATASET IS HOSTED ON HUGGING FACE (GATED ACCESS)**
> To preserve data integrity and prevent unauthorized scraping or AI model degradation, the complete production corpus is hosted exclusively on Hugging Face.
> 
> **[🔗 Click Here to Access the Full Dataset on Hugging Face](https://huggingface.co)**

## 📌 Project Overview
Sylheti is categorized as a low-resource language with a limited digital footprint. This project bridges the technological gap by building a highly structured multilingual parallel corpus. It is uniquely designed to support **AI and LLM training**, Machine Translation (MT) models, cross-lingual tokenizers, and dialectal analysis tools by mapping phonetic variations and traditional scripts across major global language families.

## 🚨 Ethical Plea & Strict Usage Notice
Aligning a severely low-resource language like Sylheti with four high-resource languages (Bangla, English, Russian, German) across different language families requires immense manual, syntactic, and computational effort. 

Creating this sequence alignment—matching precise semantic equivalence, dialectal variations, and traditional Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) script—is exceptionally complex and labor-intensive. 

**Please respect this grueling linguistic work:**
- Do **NOT** scrape, republish, or commercialize this dataset without explicit attribution.
- Unauthorized text-scraping or utilizing this schema without citing the author is strictly prohibited under the CC BY-NC 4.0 license.

## 📂 Repository Contents (Sample)
This GitHub repository contains **Sample Data (50 entries each)** to allow researchers and developers to test Python pipelines, tokenizers, and alignment scripts:

- **`data/parallel_sentences_showcase.tsv`**: 50 sample parallel sentence alignments across 5 languages (10 Columns).
- **`data/lexicon_showcase.tsv`**: 50 sample vocabulary entries with POS and metadata (11 Columns).

### 📐 Data Schema & Integrity
- **File Format:** TSV (Tab-Separated Values), UTF-8 Encoded.
- **Zero-Hallucination Policy:** Any unverified or missing script data (specifically for ancient Syloti Nagri conjuncts) are intentionally left blank (`NaN` or `Null`) to prevent AI model degradation and maintain 100% precision.

### 📊 Data Preview (Structure)

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Bangla (Standard) | English (Standard) | Russian (Русский) | German (Deutsch) | Domain | Register | POS |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1.1** | *tai* | তাই | ꠔꠣꠁ | সে (মহিলা) | She | Она | Sie | general | informal | pronoun |
| **1.2** | *tai one zaibo gi* | তাই অনে যাইবো গি | ꠔꠣꠁ ꠅꠘꠦ ꠎꠣꠁꠛꠦꠣ ꠉꠤ | সে এখন চলে যাবে। | She will leave now. | Она сейчас уйдет. | Sie wird jetzt gehen. | daily_life | informal | NaN |

## 📥 Data Loading Example (Python)
Always set `sep='\t'` and `encoding='utf-8'` when reading the `.tsv` files to prevent text corruption:

```python
import pandas as pd

# Load showcase parallel sentences
df = pd.read_csv('data/parallel_sentences_showcase.tsv', sep='\t', encoding='utf-8')
print(df.head())
```
