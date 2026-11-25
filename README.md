# Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP

![License](https://shields.io)
![Domain](https://shields.io)

Welcome to the **first structured 5-way multilingual parallel corpus** for the **Sylheti (syl)** language, engineered by a native Linguistics student. This dataset bridges Sylheti with four major global high-resource languages spanning **three distinct language families** (Indo-Aryan, Germanic, and Slavic) to support Computational Linguistics (CL), Natural Language Processing (NLP) research, and Large Language Model (LLM) fine-tuning.

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
- Do **NOT** use, redistribute, or commercialize this dataset without explicit attribution to the author.
- Unauthorized commercial scraping or utilizing this dataset for proprietary commercial AI models without permission is strictly prohibited under the **CC BY-NC 4.0** license.

## 📂 Repository Contents & Dataset Structure
This GitHub repository contains **Sample Data (50 entries each)** to allow researchers and developers to test Python pipelines, tokenizers, and alignment scripts, while the core dataset is structured in tab-separated format (`.tsv`) and hosted on Hugging Face:

- **`data/parallel_sentences_showcase.tsv`**: Sample parallel sentence alignments across 5 languages (**12 Columns**).
- **`data/lexicons_showcase.tsv`**: Sample vocabulary entries with POS and dialect/variant metadata (**13 Columns**).
- **`parallel_sentences.tsv`**: Sentence-level multilingual alignment for Machine Translation, multilingual NLP, and LLM fine-tuning.
- **`lexicons.tsv`**: Core vocabulary mapping, Sylheti variants, multilingual equivalents, linguistic metadata, and POS tagging.

### 📐 Data Schema & Integrity
- **File Format:** TSV (Tab-Separated Values), UTF-8 Encoded. Although Hugging Face automatically categorizes text-based tabular data under the generic `csv` badge, the actual production files in this repository are strictly formatted as **TSV (Tab-Separated Values)** to prevent commas in multilingual strings from corrupting the cell boundaries.
- **Pure Semantic Key (PSK) Indexing:**
  - **Lexicons:** The `lexicons.tsv` dataset uses the `lXXXXX_vXX` format, where `lXXXXX` represents the Lexical Concept / Synset ID and `vXX` represents the Sylheti Variant / Synonym ID. Synonyms or regional variants belonging to the same lexical concept share the same Lexical Concept ID and receive distinct Variant IDs.
  - **Parallel Sentences:** The `parallel_sentences.tsv` dataset uses the `sXXXXX_vXX` format, where `sXXXXX` represents the Sentence-level Semantic Equivalence Group ID and `vXX` represents the Sylheti Sentence Variant / Alternative Expression ID. Alternative sentence expressions belonging to the same semantic-equivalence group share the same Sentence Group ID and receive distinct Variant IDs.
- **Controlled Linguistic Annotation Metadata:** Both core tables conclude with four strictly controlled, closed-set annotation columns (left empty `\t\t` if unverified):
  - **`Domain`**: Categorizes the thematic context (`General`, `Daily_Life`, `Food_Hospitality`, `Nature_Environment`, `Travel_Geography`, `Culture_Folklore`, `Religion_Spirituality`, `Health_Medicine`, `Commerce_Economy`, `Education_Science`, `Governance_Law`, or `Technology_Media`).
  - **`Register`**: Identifies the sociolinguistic and stylistic level (`Informal`, `Colloquial`, `Honorific`, `Formal`, `Code_Switched`, or `Literary_Nagri`).
  - **`Dialect_Region`**: Identifies the regional or diaspora variety (`Pan-Sylheti`, `Sylhet_Sadar`, `Sunamganj`, `Habiganj`, `Moulvibazar`, `Barak_Valley`, or `Diaspora_UK`).
  - **`Variant_Type`**: Classifies the nature of the Sylheti variant (`Base`, `Regional_Lexical`, `Phonological`, `Morphological`, or `Register_Honorific`).
- **Zero-Hallucination Policy:** Missing or unverified linguistic data must be left **completely empty** (represented by consecutive tabs `\t\t` in the raw file). Literal placeholders such as `NaN`, `Null`, or `N/A`, as well as fabricated linguistic forms, are strictly prohibited. This prevents tokenizer pollution and ensures clean parsing for downstream AI/NLP pipelines such as Pandas and Hugging Face.

### 📊 Data Preview (Lexicons & Sentence Structure)

**Lexicon Schema Preview (13 Columns):**

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Bangla (Standard) | English (Standard) | Russian (Русский) | German (Deutsch) | Domain | Register | POS | Dialect_Region | Variant_Type |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **l00001_v01** | *tai* | তাই | ꠔꠣꠁ | সে (স্ত্রীলিঙ্গ) | She | Она | Sie | General | Informal | Pronoun | Pan-Sylheti | Base |

**Parallel Sentence Schema Preview (12 Columns):**

| Index | Sylheti (Romanized) | Sylheti (Bangla Script) | Syloti Nagri (ꠍꠤꠟꠐꠤ ꠘꠣꠉꠞꠤ) | Bangla (Standard) | English (Standard) | Russian (Русский) | German (Deutsch) | Domain | Register | Dialect_Region | Variant_Type |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **s00001_v01** | *tai oxon zaibogi* | তাই অখন যাইবগি | ꠔꠣꠁ ꠅꠈꠘ ꠎꠣꠁꠛꠉꠤ | সে এখন চলে যাবে। | She will leave now. | Она сейчас уйдет. | Sie wird jetzt gehen. | Daily_Life | Informal | Pan-Sylheti | Base |

## 🚀 Future Roadmap & Core Goals
- **Scale toward 10,000–20,000+ Parallel Sentences:** Continually expand dataset rows to establish a world-class digital preservation corpus for AI.
- **Granular Dialect & Variant Expansion:** Expand annotated coverage across sub-regional and diaspora varieties (`Sylhet_Sadar`, `Sunamganj`, `Habiganj`, `Moulvibazar`, `Barak_Valley`, and `Diaspora_UK`) using the established `Dialect_Region` and `Variant_Type` metadata columns.
- **Phonetic & Acoustic Metadata (IPA):** Develop a separate `phonetic_metadata.tsv` relational table mapped directly via the **Pure Semantic Key (PSK)** indices (`lXXXXX_vXX` / `sXXXXX_vXX`). This will integrate IPA transcriptions to preserve Sylheti tonogenesis & VOT, paving the way for advanced TTS & ASR technologies.
- **Acoustic Audio Alignment:** Collect high-fidelity spoken data for Automatic Speech Recognition (ASR) and Speech Synthesis (TTS).
- **Nagri OCR Pipeline:** Build character recognition models for ancient Nagri manuscripts (Pothi literature).

## 🤝 Contributing
This repository and corpus are maintained with strict access controls to preserve dataset integrity and prevent AI degradation.
- **Strict Policy:** External Pull Requests or dataset edits are accepted strictly by invitation only.
- To request research access or collaborate, contact the maintainer directly.

## 🧑‍💻 About the Author
I am **Fahim Ahmed** (cited academically as **Ahmed, Fahim**), an undergraduate Linguistics student at **Kursk State University, Russia**, and a **native Sylheti speaker**. As an aspiring Computational Linguist, I am independently building this dataset to preserve, revitalize, and digitize the Sylheti language using modern AI pathways and LLM architectures.

## 📜 License
This dataset is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**. You are free to share and adapt the material for **non-commercial purposes**, provided you give appropriate credit. All commercial rights are reserved by the author (**Fahim Ahmed**).

## 📋 Citation
If you use this dataset, lexicon, or parallel corpus in your research, software, or AI models, please cite it exactly as follows:

```bibtex
@misc{ahmed2026sylheti,
  author       = {Ahmed, Fahim},
  title        = {Sylheti-Bangla-English-Russian-German Parallel Corpus for NLP},
  year         = {2026},
  version      = {1.0.0},
  publisher    = {Hugging Face},
  url          = {https://huggingface.co}
}
```
