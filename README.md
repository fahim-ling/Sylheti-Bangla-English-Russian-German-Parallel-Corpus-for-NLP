# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)
![Domain: NLP / Computational Linguistics](https://img.shields.io/badge/Domain-NLP%20%2F%20CL-blue)

Welcome to the first open-source multi-lingual parallel corpus for the **Sylheti** language, designed to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and **La[...]

## 📌 Project Overview
Sylheti is categorized as a low-resource language with a limited digital footprint. This project bridges the technological gap by building a highly structured multi-lingual parallel corpus. It is uniq[...]

## 📂 Dataset Structure & Preview
* **Format:** CSV / Google Sheets (UTF-8 Encoded)
* **Project Files:** 
  * `parallel_sentences.csv`: For sentence-level mappings, Machine Translation, and **LLM fine-tuning**.
  * `lexicon.csv`: For single words, vocabulary, and short phrases.
* **Data Integrity Note:** Missing or unverified script data (e.g., unverified Nagri inputs) are intentionally left blank (`Null/NaN`) to ensure maximum dataset precision and prevent model degrada[...]
* **Dialectal Indexing:** Sub-regional variations (e.g., Sylhet Sadar, Sunamganj, Habiganj) are mapped using a structured decimal numbering system (`1.1`, `1.2`) linked to a single semantic meanin[...]

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Bangla (Standard) | English (Standard) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Russian (Русский) | German (Deutsch) | Domain | Register |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1.1** | *Ami okhon zaimugi* | আমি অখন যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠀꠈꠘ ꠎꠣꠁꠝꠥꠉꠤ | Я сей[...]
| **1.2** | *Ami one zaimugi* | আমি অনে যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠅꠘ ꠎꠣ ꠝꠥꠉꠤ | Я сейчас у[...]
| **1.3** | *Ami akhon zaimuga* | আমি আখন যাইমুগা | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠀꠈꠘ ꠎꠣꠁꠝꠥꠉꠣ | Я сей[...]

## 🚀 Future Roadmap & Core Goals
- **Scale to 10,000+ Parallel Sentences:** Continually expand the dataset rows to establish a world-class digital preservation corpus for AI.
- **Granular Dialect Mapping:** Systematically categorize sub-regional dialects (e.g., Sylhet Sadar, Sunamganj, Habiganj, Moulvibazar) using precise metadata tags.
- **German Language Integration:** Complete parallel translation vectors for German to allow advanced syntactic and structural analysis.
- **Acoustic Audio Alignment:** Collect high-fidelity spoken data for Automatic Speech Recognition (ASR) and Speech Synthesis (TTS).

## 🧑‍💻 About the Author
I am an undergraduate Linguistics student at **Kursk State University, Russia**, and a **native Sylheti speaker**. As an aspiring Computational Linguist, I am independently building this dataset t[...]

Author: Ahmed Fahim

## 📥 Download & Usage
- The dataset files (`parallel_sentences.csv`, `lexicon.csv`) are stored in this repository under the `data/` directory. You can download them directly from GitHub or use `git clone` to clone the repository.
- Encoding: UTF-8. Verify encoding when loading into tools (for example, with pandas: `pd.read_csv('parallel_sentences.csv', encoding='utf-8')`).
- Citation and attribution are required under the CC-BY-4.0 license (see LICENSE file for full text).

## 🤝 Contributing
This repository is maintained privately at project start. Contributions are accepted only from explicitly invited collaborators (e.g., close family members). Do not submit changes without prior permission. To request access, contact the maintainer; unsolicited PRs will be closed.

## 📜 License
This project and the dataset are licensed under the **Creative Commons Attribution 4.0 International License (CC-BY-4.0)**. 
You are free to share and adapt the material for any purpose, even commercially, as long as you give appropriate credit.

## 📝 Citation
If you use this dataset or corpus in your research, software, or project, please cite it using the following format:

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
