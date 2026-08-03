# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)
![Domain: NLP / Computational Linguistics](https://img.shields.io/badge/Domain-NLP%20%2F%20CL-blue)

Welcome to the first open-source multi-lingual parallel corpus for the **Sylheti** language, designed to support Computational Linguistics (CL) and Natural Language Processing (NLP) research.

## 📌 Project Overview
Sylheti is categorized as a low-resource language with a limited digital footprint. This project bridges the technological gap by building a highly structured multi-lingual parallel corpus. It is uniquely designed to train Machine Translation (MT) models, cross-lingual tokenizers, and dialectal analysis tools by mapping phonetic variations and traditional scripts across major global language families.

## 📂 Dataset Structure & Preview
* **Format:** CSV / Google Sheets (UTF-8 Encoded)
* **Data Integrity Note:** Missing or unverified script data (e.g., unverified Nagri inputs) are intentionally left blank (`Null/NaN`) to ensure maximum dataset precision and prevent model degradation from incorrect annotations.
* **Dialectal Indexing:** Sub-regional variations (e.g., Sylhet Sadar, Sunamganj, Habiganj) are mapped using a structured decimal numbering system (`1.1`, `1.2`) linked to a single semantic meaning.

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Bangla (Standard) | English (Standard) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Russian (Русский) | German (Deutsch) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1.1** | *Ami okhon zaimugi* | আমি অখন যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠀꠈꠘ ꠎꠣꠁꠝꠥꠉꠤ | Я сейчас уйду. | Ich gehe jetzt. |
| **1.2** | *Ami one zaimugi* | আমি অনে যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠅꠘꠦ ꠎꠣꠁꠝꠥꠉꠤ | Я сейчас уйду. | Ich gehe jetzt. |
| **1.3** | *Ami akhon zaimuga* | আমি আখন যাইমুগা | আমি এখন চলে যাব। | I will leave now. | ꠀꠝꠤ ꠀꠈꠘ ꠎꠣꠁꠝꠥꠉꠣ | Я сейчас уйду. | Ich gehe jetzt. |

## 🚀 Future Roadmap & Core Goals
- **Scale to 10,000+ Parallel Sentences:** Continually expand the dataset rows to establish a world-class digital preservation corpus.
- **Granular Dialect Mapping:** Systematically categorize sub-regional dialects (e.g., Sylhet Sadar, Sunamganj, Habiganj, Moulvibazar) using precise metadata tags.
- **German Language Integration:** Complete parallel translation vectors for German to allow advanced syntactic and structural analysis.
- **Acoustic Audio Alignment:** Collect high-fidelity spoken data for Automatic Speech Recognition (ASR) and Speech Synthesis (TTS).

## 🧑‍💻 About the Author
I am an undergraduate Linguistics student at **Kursk State University, Russia**, and a **native Sylheti speaker**. As an aspiring Computational Linguist, I am independently building this dataset to preserve, revitalize, and digitize the Sylheti language using modern computational methods.

## 📜 License
This project and the dataset are licensed under the **Creative Commons Attribution 4.0 International License (CC-BY-4.0)**. 
You are free to share and adapt the material for any purpose, even commercially, as long as you give appropriate credit.

## 📝 Citation
If you use this dataset or corpus in your research, software, or project, please cite it using the following format:

### APA Format
Fahim, A. (2026). Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP. GitHub Repository. https://github.com/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP

### BibTeX Format
```bibtex
@misc{fahim2026sylheti,
  author = {Ahmed Fahim},
  title = {Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub Repository},
    howpublished = {\url{https://github.com/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP}}
}
