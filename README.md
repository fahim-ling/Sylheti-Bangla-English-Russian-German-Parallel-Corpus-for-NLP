# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-blue.svg)
![Domain](https://img.shields.io/badge/Domain-NLP%20%2F%20Computational%20Linguistics-success.svg)

Welcome to the **first open-source multilingual parallel corpus** for the **Sylheti (syl)** language, engineered by a native Linguistics student. This dataset bridges Sylheti with four major global high-resource languages spanning **three distinct language families** (Indo-Aryan, Germanic, and Slavic) to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and Large Language Model (LLM) fine-tuning.


> 🚨 **NOTICE: FULL DATASET IS HOSTED ON HUGGING FACE (GATED ACCESS)**
> To preserve data integrity and prevent unauthorized scraping or AI model degradation, the complete production corpus is hosted exclusively on Hugging Face.
> 
> **[🔗 Click Here to Access the Full Dataset on Hugging Face](https://huggingface.co/datasets/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP)**


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

### 📊 Combined Data Preview (Lexicon & Sentence Structure)

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Bangla (Standard) | English (Standard) | Russian (Русский) | German (Deutsch) | Domain | Register | POS |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1.1** | *tai* | তাই | ꠔꠣꠁ | সে (মহিলা) | She | Она | Sie | General | Informal | Pronoun |
| **1.2** | *tai oxon zaibogi* | তাই অখন যাইবগি | ꠔꠣꠁ ꠅꠈꠘ ꠎꠣꠁꠛꠉꠤ | সে এখন চলে যাবে। | She will leave now. | Она сейчас уйдет. | Sie wird jetzt gehen. | Daily Life | Informal | NaN |


## 🧑‍💻 About the Author
I am **Fahim Ahmed** (cited academically as **Ahmed Fahim**), an undergraduate Linguistics student at **Kursk State University, Russia**, and a **native Sylheti speaker**. As an aspiring Computational Linguist, I am independently building this dataset to preserve, revitalize, and digitize the Sylheti language using modern AI pathways and LLM architectures.


## 🤝 Contributing
This repository and corpus are maintained with strict access controls to preserve dataset integrity and prevent AI degradation.
- **Strict Policy:** External Pull Requests or dataset edits are accepted strictly by invitation only.
- To request research access or collaborate, contact the maintainer directly.


## 🚀 Future Roadmap & Core Goals
- **Scale to 10,000+ Parallel Sentences:** Continually expand dataset rows to establish a world-class digital preservation corpus for AI.
- **Granular Dialect Mapping:** Systematically categorize sub-regional dialects (e.g., Sylhet Sadar, Sunamganj, Habiganj, Moulvibazar) using precise metadata tags.
- **Phonetic & Acoustic Metadata (IPA):** Develop a separate phonetic_metadata.tsv relational table mapped via strict decimal indices. This will integrate IPA transcriptions to preserve Sylheti tonogenesis & VOT, paving the way for advanced TTS & ASR technologies.
- **Acoustic Audio Alignment:** Collect high-fidelity spoken data for Automatic Speech Recognition (ASR) and Speech Synthesis (TTS).
- **Nagri OCR Pipeline:** Build character recognition models for ancient Nagri manuscripts (Pothi literature).


## 📥 Data Loading Example (Python)
Always set `sep='\t'` and `encoding='utf-8'` when reading the `.tsv` files to prevent text corruption:

```python
import pandas as pd

# Load lexicon
lexicon_df = pd.read_csv('data/lexicon.tsv', sep='\t', encoding='utf-8')

# Load showcase parallel sentences
parallel_df = pd.read_csv('data/parallel_sentences_showcase.tsv', sep='\t', encoding='utf-8')

print(lexicon_df.head())
print(parallel_df.head())
```
