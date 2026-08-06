# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)
![Domain: NLP / Computational Linguistics](https://img.shields.io/badge/Domain-NLP%20%2F%20CL-blue)

Welcome to the first open-source multi-lingual parallel corpus for the Sylheti language, designed to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and large-scale language model work (e.g., model evaluation and fine-tuning).

## 📌 Project Overview
Sylheti is categorized as a low-resource language with a limited digital footprint. This project bridges the technological gap by building a highly structured multi-lingual parallel corpus. It is unique in providing aligned sentence- and word-level data across Sylheti (romanized and native scripts), Standard Bangla, English, Russian and German to support research and practical NLP applications.

## 📂 Dataset Structure & Preview
- Format: CSV / Google Sheets (UTF-8 Encoded)
- Project Files:
  - `parallel_sentences.csv`: Sentence-level mappings for machine translation, cross-lingual experiments, and LLM fine-tuning.
  - `lexicon.csv`: Word-level and short-phrase lexicon entries with part-of-speech tags and glosses where available.
- Data Integrity Note: Missing or unverified script data (for example, unverified Syloti Nagri inputs) are intentionally left blank (`Null/NaN`) to ensure maximum dataset precision and to prevent downstream model degradation.
- Dialectal Indexing: Sub-regional variations (e.g., Sylhet Sadar, Sunamganj, Habiganj, Moulvibazar) are mapped using a structured decimal numbering system (`1.1`, `1.2`) linked to a single semantic meaning. Dialect metadata is provided in a dedicated column in the CSV files.

### Sample (first rows)

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Bangla (Standard) | English (Standard) | Syloti Nagri | Russian (Русский) | German (Deutsch) | Domain |
| :---: | :-----------------: | :---------------------: | :---------------: | :----------------: | :----------: | :---------------: | :---------------: | :----: |
| 1.1 | Ami okhon zaimugi | আমি অখন যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ | Я сейчас уйду. | Ich werde jetzt gehen. | general |
| 1.2 | Ami one zaimugi | আমি অনে যাইমুগি | আমি এখন চলে যাব। | I will leave now. | ꠍꠤꠟꠐꠤ ꠅꠘ ꠎꠣ ꠝꠥꠉꠤ | Я сейчас уйду. | Ich werde jetzt gehen. | dialectal |
| 1.3 | Ami akhon zaimuga | আমি আখন যাইমুগা | আমি এখন চলে যাব। | I will leave now. | ꠍꠤꠟꠐꠤ ꠈꠘ ꠎꠣꠁꠝꠥꠉꠣ | Я сейчас уйду. | Ich werde jetzt gehen. | dialectal |

> Note: The sample rows above are illustrative. Please consult `parallel_sentences.csv` for the complete dataset. Syloti Nagri (Nagri) columns may show as blank where script encoding or verification is pending.

## 🚀 Future Roadmap & Core Goals
- Scale to 10,000+ parallel sentences to establish a world-class digital preservation corpus for AI.
- Granular dialect mapping: systematically categorize sub-regional dialects using precise metadata tags.
- German language integration: complete parallel translation vectors for German to allow advanced syntactic and structural analysis.
- Acoustic audio alignment: collect high-fidelity spoken data for Automatic Speech Recognition (ASR) and Text-to-Speech (TTS).

## 🧑‍💻 About the Author
I am an undergraduate Linguistics student at Kursk State University, Russia, and a native Sylheti speaker. As an aspiring Computational Linguist, I am independently building this dataset to promote digital preservation and enable multilingual NLP research.

Author: Ahmed Fahim

## 📥 Download & Usage
- The dataset files (`parallel_sentences.csv`, `lexicon.csv`) are stored in this repository under the `data/` directory. You can download them directly from GitHub or use `git clone` to clone the repository.
- Encoding: UTF-8. Verify encoding when loading into tools (for example, with pandas: `pd.read_csv('parallel_sentences.csv', encoding='utf-8')`).
- Citation and attribution are required under the CC-BY-4.0 license (see LICENSE file for full text).

## 🤝 Contributing
Contributions are welcome. Please follow these steps:
1. Fork the repository.
2. Create a branch for your changes (`git checkout -b fix/my-change`).
3. Make your edits and add tests or notes where appropriate.
4. Open a Pull Request describing your change and link any relevant sources.

Please be careful with script conversions (Syloti Nagri ↔ Bangla script) and mark any unverified entries as `unverified` in the dialect/script verification column.

## 📜 License
This project and the dataset are licensed under the Creative Commons Attribution 4.0 International License (CC-BY-4.0).
A copy of the full license text is included in the repository as `LICENSE`.

## 📝 Citation
If you use this dataset or corpus in your research, software, or project, please cite it using the following formats.

### APA Format
Ahmed Fahim. (2026). Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP. GitHub Repository. https://github.com/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP

### BibTeX Format
```bibtex
@misc{fahim2026sylheti,
  author       = {Ahmed Fahim},
  title        = {Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP},
  year         = {2026},
  publisher    = {GitHub},
  url          = {https://github.com/fahim-ling/Sylheti-Bangla-English-Russian-German-Parallel-Corpus-for-NLP},
}
```

---

If you want, I can also:
- create a new branch and open a pull request with this README change, or
- make additional changes like adding a `data/` folder with small README metadata files, or
- add a CONTRIBUTING.md and LICENSE file if missing.
