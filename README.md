# Unstructured Data Analysis (2026-2) — Programming Materials

**Institution:** Hanyang University, Department of Data Science
**Professor:** Misuk Kim
**Teaching Assistant:** Hojin Son (hojinson@hanyang.ac.kr)

This repository holds the **programming session notebooks and assignments** for the course.
Lecture videos and slides are distributed through the LMS; this repository only contains the hands-on material.

---

## 📅 Programming sessions (2026-2)

| # | Date | Topic | Assignment |
|---|---|---|---|
| 1 | Sep 21 | Text Preprocessing | Programming Assignment 1 |
| 2 | Sep 28 | Text Representation 1 | Programming Assignment 2 |
| 3 | Oct 12 | Text Representation 2 | Programming Assignment 3 |
| 4 | Oct 19 | Dimensionality Reduction | Programming Assignment 4 |
| 5 | Nov 9 | Document Classification | Programming Assignment 5 |
| 6 | Nov 23 | Sentiment Analysis | Programming Assignment 6 |

Midterm exam: **Oct 26** · Final exam: **Dec 14**

---

## 📂 Week 3 — Text Preprocessing (Sep 21)

| Notebook | Open |
|---|---|
| 1. Text Preprocessing Process | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week03-text-preprocessing/01_text_preprocessing.ipynb) |
| 2. Visualization | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week03-text-preprocessing/02_visualization.ipynb) |
| **Assignment 1** (due Sep 28, 23:59) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week03-text-preprocessing/03_assignment1_text_preprocessing.ipynb) |

**Contents**

- `01_text_preprocessing.ipynb` — sentence splitting, tokenization (`word_tokenize`, `WordPunctTokenizer`, `RegexpTokenizer`), stop-word removal, stemming vs. lemmatization, POS tagging, NER
- `02_visualization.ipynb` — word-frequency graphs and word clouds on the *Moby Dick* corpus
- `03_assignment1_text_preprocessing.ipynb` — fill-in-the-blank assignment on the Twitter Entity Sentiment dataset (100 points)
- `data/` — `twcs.csv` (Twitter entity sentiment), `whale_mask.png` (word-cloud mask)

---

## 💻 How to use the notebooks

1. Click the **Open In Colab** badge above. You do **not** need a GitHub account — a Google account is enough.
2. In Colab, choose **File ▸ Save a copy in Drive**. Edits made without saving a copy are lost.
3. Run the cells from top to bottom with **Shift + Enter**. Always run the **Setup** cell first — it downloads the NLTK resources.
4. If a cell hangs, use **Runtime ▸ Restart session** and run the Setup cell again.

Requirements are handled inside the notebooks (`nltk`, `wordcloud`, `pandas`, `matplotlib`).
The datasets are downloaded automatically from this repository, so **Google Drive mounting is not required**.

---

## 📝 Assignment submission

Rename your notebook to `Assignment_N_YourName_StudentID.ipynb` (e.g. `Assignment_1_HongGilDong_2026123456.ipynb`),
run it once from top to bottom so that all outputs are visible, and submit the `.ipynb` file through the LMS.

---

## 📊 Data sources

- Twitter Entity Sentiment Analysis — https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis
- Moby Dick — Project Gutenberg sample bundled with NLTK (`nltk.corpus.gutenberg`)

---

## 🙏 Acknowledgement

The programming materials are based on those prepared by the previous teaching assistant,
[Min Joo Son](https://github.com/ming9oori/2025-2-Unstructured-Data-Analysis) (2025-2), updated for the current NLTK and Colab environment.
