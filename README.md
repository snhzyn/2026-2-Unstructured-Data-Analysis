# Unstructured Data Analysis (2026-2) - Programming Materials

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
| 2 | Sep 28 | Text Representation I - Classic Method | Programming Assignment 2 |
| 3 | Oct 12 | Text Representation II - Distributed Method | Programming Assignment 3 |
| 4 | Oct 19 | Dimensionality Reduction | Programming Assignment 4 |
| 5 | Nov 9 | Document Classification | Programming Assignment 5 |
| 6 | Nov 23 | Sentiment Analysis | Programming Assignment 6 |

Midterm exam: **Oct 26** · Final exam: **Dec 14**

---

## 📂 Week 3 - Text Preprocessing (Sep 21)

| Notebook | Open |
|---|---|
| 1. Text Preprocessing Process | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week03-text-preprocessing/01_text_preprocessing.ipynb) |
| 2. Visualization | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week03-text-preprocessing/02_visualization.ipynb) |
| **Assignment 1** (due Sep 28, 23:59) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week03-text-preprocessing/03_assignment1_text_preprocessing.ipynb) |

**Contents**

- `01_text_preprocessing.ipynb` : sentence splitting, tokenization (`word_tokenize`, `WordPunctTokenizer`, `RegexpTokenizer`), stop-word removal, stemming vs lemmatization, POS tagging, NER
- `02_visualization.ipynb` : word-frequency graphs and word clouds on the *Moby Dick* corpus
- `03_assignment1_text_preprocessing.ipynb` : fill-in-the-blank assignment on the Twitter Entity Sentiment dataset (100 points)
- `data/` : `twcs.csv` (Twitter entity sentiment), `whale_mask.png` (word-cloud mask)

**Data sources**

- Twitter Entity Sentiment Analysis : https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis
- Moby Dick : Project Gutenberg sample bundled with NLTK (`nltk.corpus.gutenberg`)

---

## 📂 Week 4 - Text Representation I : Classic Method (Sep 28)

Covers lecture **4-1 Text Representation I - Classic Method** (Bag of Words · Word Weighting · N-Grams).

| Notebook | Open |
|---|---|
| 1. Bag of Words | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week04-text-representation-1/01_bag_of_words.ipynb) |
| 2. Word Weighting & N-Grams | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week04-text-representation-1/02_word_weighting_and_ngrams.ipynb) |
| **Assignment 2** (due Oct 5, 23:59) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/snhzyn/2026-2-Unstructured-Data-Analysis/blob/main/week04-text-representation-1/03_assignment2_text_representation.ipynb) |

**Contents**

- `01_bag_of_words.ipynb` : term-document matrix by hand (binary vs frequency), word order is lost,
  preprocessing and stop words, the matrix on 2,000 reviews, `CountVectorizer`, sparsity,
  Korean text with KoNLPy (`Okt`)
- `02_word_weighting_and_ngrams.ipynb` : term frequency (the Shakespeare table rebuilt from NLTK),
  document frequency and IDF, TF-IDF with the lecture's worked example, SMART variants
  (`sublinear_tf` / `use_idf` / `norm`), n-grams, cosine similarity
- `03_assignment2_text_representation.ipynb` : fill-in-the-blank assignment on the Twitter Entity
  Sentiment dataset from Assignment 1 - term-document matrix, df/idf, TF-IDF, n-grams,
  cosine similarity (100 points)
- `data/` : `daum_movie_review.csv` (Korean movie reviews). The assignment reuses
  `week03-text-preprocessing/data/twcs.csv`.

**Data sources**

- Movie Reviews (English) : `nltk.corpus.movie_reviews` (Pang & Lee)
- Shakespeare plays : `nltk.corpus.gutenberg`
- Daum movie reviews (Korean) : collected for this course

---

## 💻 How to use the notebooks

1. Click the **Open In Colab** link above. You do **not** need a GitHub account; a Google account is enough.
2. In Colab, choose **File ▸ Save a copy in Drive**. Edits made without saving a copy are lost.
3. Run the cells from top to bottom with **Shift + Enter**. Always run the **Setup** cell first. It downloads the NLTK resources.
4. If a cell hangs, use **Runtime ▸ Restart session** and run the Setup cell again.

Requirements are handled inside the notebooks (`nltk`, `wordcloud`, `pandas`, `matplotlib`).
The datasets are downloaded automatically from this repository, so **Google Drive mounting is not required**.

---

## 📝 Assignment submission

Rename your notebook to `Assignment_N_YourName_StudentID.ipynb` (e.g. `Assignment_1_HongGilDong_2026123456.ipynb`).
**Run it once** from top to bottom so that all outputs are visible, and submit the `.ipynb` file through the LMS.

---

## 📄 Usage

These materials are prepared for students of *Unstructured Data Analysis* (2026-2) at
Hanyang University. They may be used freely for study within the course.
Redistribution or use outside the course requires permission from the instructor.
The datasets belong to their original sources listed in each week's section.

© 2026 Industrial Data Science Lab (IDSL), Hanyang University

---

## 🙏 Acknowledgement

Special thanks to **Minjoo Son**, a Ph.D. student in our lab (IDSL) and a former teaching
assistant for this course. The structure of these programming sessions, the choice of
examples, and much of the code are hers, updated here for the current NLTK and Colab
environment. Her careful preparation made this year's materials possible.
