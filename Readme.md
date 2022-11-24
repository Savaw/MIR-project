# Modern Information Retrieval Course Project

- Fall 2021

## Phase 1

In this phase, we implement an information retrieval system for both English and Persian.


### Data

Two corpora are used in this phase, one is in English, and one is in Persian. Corpora are located in the `phase1-data` directory. The English texts are from the news, and the Persian texts are from Wikipedia.

### Part 1: Preprocessing

This part includes actions to preprocess the text, including removing punctuations, normalization, tokenization, stemming, removing stop words, etc.

### Part 2: Indexing

In this part, we create indexes on the preprocessed text. Two types of indexing are used: Positional indexing and Bigram indexing.
Bigram

### Part 3: Compression

In this section, compression is performed on the indexes. Two compression method is implemented namely Variable Byte compression and Gamma Code compression.

### Part 4: Query Correction

In this part, the query is corrected by replacing misspelled words with the best alternative. We use Jaccard score to find options. The word with minimum edit distance is used to replace the misspelled word.

---
## Phase 2

In this phase, our goal is to build an error correction system to fix the errors in a query.

### Data

This phase's data is split into three directories. The first part is the "corpus," which includes texts whose tokens are used to build the model. The second part is the "training set," which includes pair of phrases with an edit distance. The third part is "dev set," which includes phrases, their correct form (ground truth), and the corrected version by google.
The data can be downloaded from [here](https://drive.google.com/file/d/17ukKiVAYtbBuL_zI8_2IhZ8uzxkMJdPs/view).

### Part 1: Language Model

In this part, the prior distributions of unigrams and bigrams are calculated using MLE.

### Part 2: Edit Probability Model

This model calculated the probability of an error in a query.

### Part 3: Candidate Generator

This part generated candidates to replace errors by getting the initial query.

### Part 4: Candidate Scorer

In this section, candidates are scored using the language model and edit probability distance.

----
## Phase 3

In this phase, we implement some classification and clustering algorithms on text. We have also implemented a crawler.

### Data

[AG News](https://www.kaggle.com/amananandrai/ag-news-classification-dataset?select=train.csv) dataset is used in this phase.

### Part 1: Classification

In this section, three classification algorithms, including Naive Bayes, SVM, and KNN, are trained and evaluated on text data.

### Part 2: Clustering

Two clustering algorithms, namely K-means and agglomerative clustering, are implemented in this part.

### Part 3: Crawler

In this part, a crawler on the ResearchGate website is implemented.

