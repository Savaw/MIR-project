# Modern Information Retrieval Cource Project

Fall 2021

## Phase 1

In this phase we implement an information retrieval system for both English and Persian language.


### Data

Two corpus are used in this phase, one is in English, and one is in Persian. Corpora are located in `phase1-data`. The English texts are from news, and the Persian texts are from Persian Wikipedia.

### Part 1: Preprocessing

This part include actions to preprocesse the text including removing punctuations, normalization, tokenization, stemming, removing stop words, etc.

### Part 2: Indexing

In this part, we create indexes on the preprocessed text. Two type of indexing is used: Positional indexing and Bigram indexing.
Bigram

### Part 3: Compression

In this section, compression is performed on the indexes. Two compression method is implemented, namely Variable Byte compression and Gamma Code compression.

### Part 4: Query Correction

In this part the query is corrected by replacing misspelled words with best alternative. We use jaccard score to find options. The word with minimum edit distance is used to replace the misspelled word.

## Phase 2

In this phase our goal is to build an error correction system to fix the errors in a query.

### Data

Data has three parts. The first part is the "corpus" which we use its token to build the model. The second part is the "training set" which include pair of phrases with an edit distance. The third part is "dev set" which include phrases, their correct form (ground truth), and the corrected version by google.
It can be downloaded from [here](https://drive.google.com/file/d/17ukKiVAYtbBuL_zI8_2IhZ8uzxkMJdPs/view).

### Part 1: Language Model

### Part 2: Edit Probability Model

### Part 3: Candidate Generator

### Part 4: Candidate Scorer

## Phase 3

In this phase, we implement some classification and clustering algorithms on text. We have also implemented a crawler.

### Data

[AG News](https://www.kaggle.com/amananandrai/ag-news-classification-dataset?select=train.csv) dataset is used in this phase.

### Part 1: Classification

In this section, three classification algorithms including Naive Bayes, SVM, and KNN are trained and evaluated on text data.

### Part 2: Clustering

Two clustering algorithms, namely K-means and agglomerative clustering is implemented in this part.

### Part 3: Crawler

In this part, a crawler on ResearchGate website is implemented.
