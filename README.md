# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)
![Domain: NLP / Computational Linguistics](https://img.shields.io/badge/Domain-NLP%20%2F%20CL-blue)

Welcome to the first open-source multilingual parallel corpus for the **Sylheti** language, designed to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and **Large Language Model (LLM) training**.

## 📌 Project Overview
Sylheti is categorized as a low-resource language with a limited digital footprint. This project bridges the technological gap by building a highly structured multilingual parallel corpus. It is uniquely designed to support **AI and LLM training**, Machine Translation (MT) models, cross-lingual tokenizers, and dialectal analysis tools by mapping phonetic variations and traditional scripts across major global language families.

## 📂 Dataset Structure & Preview
* **Format:** TSV (Tab-Separated Values) / Mobile WPS Spreadsheet Compatible (UTF-8 Encoded)
* **Core Files:** 
  * `parallel_sentences.tsv`: Sentence-level mapping for Machine Translation and **LLM fine-tuning**.
  * `lexicon.tsv`: Single words, core vocabulary, and short phrases.
* **Data Integrity:** Unverified or missing script data (e.g., uncertain Nagri inputs) are intentionally left blank (`Null/NaN`) to maintain high precision and prevent AI model degradation.
* **Dialect Mapping:** Sub-regional variations (e.g., Sylhet Sadar, Sunamganj) sharing the same semantic meaning are linked using a structured decimal index (e.g., `1.1`, `1.2`).

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Bangla (Standard) | English (Standard) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Russian (Русский) | German (Deutsch) | Domain | Register |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1.1** | *Ami okhon zaimugi* | আমি অখন যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠀꠈꠘ ꠎꠣꠁꠝꠥꠉꠤ | Я сейчас уйду. | Ich gehe jetzt. | daily_life | informal |
| **1.2** | *Ami one zaimugi* | আমি অনে যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠅꠘꠦ ꠎꠣꠁꠝꠥꠉꠤ | Я сейчас уйду. | Ich gehe jetzt. | daily_life | informal |
| **1.3** | *Ami akhon zaimuga* | আমি আখন যাইমুগা | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠀꠈꠘ ꠎꠣꠁꠝꠥꠉꠣ | Я сейчас уйду. | Ich gehe jetzt. | daily_life | informal |

## 📥 Download & Usage
The dataset files (`parallel_sentences.tsv`, `lexicon.tsv`) are stored in this repository under the `data/` directory. You can download them directly from GitHub or use `git clone` to clone the repository.

* **Encoding:** UTF-8. 
* **Data Loading Example (Python/Pandas):** Always verify encoding when loading into tools to prevent text corruption:
  ```python
  import pandas as pd
  df = pd.read_csv('parallel_sentences.csv', encoding='utf-8')
  ```
* **Attribution:** Citation and attribution are strictly required under the CC-BY-4.0 license framework (see `LICENSE` file for full text).

## 🤝 Contributing
This repository is maintained privately at project start. Contributions are accepted only from explicitly invited collaborators (e.g., close family members and verified academic peers). 

* **Strict Policy:** Do not submit changes without prior written permission. 
* To request access or collaborate, contact the maintainer directly. Unsolicited Pull Requests (PRs) or unauthorized issues will be immediately closed without review.

## 🚀 Future Roadmap & Core Goals
- **Scale to 10,000+ Parallel Sentences:** Continually expand the dataset rows to establish a world-class digital preservation corpus for AI.
- **Granular Dialect Mapping:** Systematically categorize sub-regional dialects (e.g., Sylhet Sadar, Sunamganj, Habiganj, Moulvibazar) using precise metadata tags.
- **German Language Integration:** Complete parallel translation vectors for German to allow advanced syntactic and structural analysis.
- **Acoustic Audio Alignment:** Collect high-fidelity spoken data for Automatic Speech Recognition (ASR) and Speech Synthesis (TTS).

## 🧑‍💻 About the Author
I am an undergraduate Linguistics student at **Kursk State University, Russia**, and a **native Sylheti speaker**. As an aspiring Computational Linguist, I am independently building this dataset to preserve, revitalize, and digitize the Sylheti language using modern computational methods.

## 📜 License & Unauthorized Use Notice
This project and the dataset are licensed under the **Creative Commons Attribution 4.0 International License (CC-BY-4.0)**. You are free to share and adapt the material as long as appropriate credit is given.

⚠️ **IMPORTANT NOTICE:** Unauthorized commercial distribution, text-scraping without explicit attribution, or copying this parallel data schema without mentioning the author is strictly prohibited. Legal actions and standard GitHub DMCA Takedown notices will be filed against any web scraping tools, companies, or individuals found misusing this corpus or publishing it without proper academic citation.

## 📝 Citation
If you use this dataset, lexicon, or parallel corpus in your research, software, or AI models, please cite it exactly as follows:

### APA Format
Ahmed Fahim. (2026). Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP. GitHub Repository. https://github.com/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP

### BibTeX Format
```bibtex
@misc{fahim2026sylheti,
  author       = {{Ahmed Fahim}},
  title        = {Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP},
  year         = {2026},
  publisher    = {GitHub},
  howpublished = {\url{https://github.com/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP}}
}
```
