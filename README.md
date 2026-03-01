# 🏦 Bank Review Analysis

### Semantic Clustering & Sentiment Analysis using NLP

------------------------------------------------------------------------

## 📌 Project Summary

This project analyzes **customer reviews of Indian banks** scraped from
**MouthShut.com** and applies advanced NLP techniques including:

-   Semantic chunking
-   Text embeddings
-   Sentiment probability modeling
-   Topic aggregation
-   Factor analysis
-   Hierarchical clustering

The objective is to identify:

-   Topic-level sentiment patterns
-   Comparative bank positioning
-   Cluster-based similarities
-   Strategic insights (SWOT-style interpretation)

------------------------------------------------------------------------

## 🌐 Data Source

Customer reviews were obtained through web scraping from:

https://www.mouthshut.com

The dataset includes:

-   Bank name
-   Review text
-   User rating
-   Associated metadata

All reviews were processed strictly for academic and analytical
purposes.

------------------------------------------------------------------------

## 🗂 Project Structure
<img width="826" height="727" alt="image" src="https://github.com/user-attachments/assets/ff542976-4506-4907-aa9a-79e38bdf9d1c" />

------------------------------------------------------------------------

## 🔬 Methodology

### 1️⃣ Web Scraping

-   Extracted bank reviews from MouthShut.com
-   Structured into tabular dataset
-   Stored as data/final.xlsx

### 2️⃣ Text Preprocessing

-   Cleaning and normalization
-   Removal of noise
-   Preparation for embedding model

### 3️⃣ Semantic Chunking

-   Long reviews split into meaningful semantic chunks
-   Index mapping preserved\
-   Output: df_chunks_with_index.csv

### 4️⃣ Embedding Generation

-   Converted text chunks into vector embeddings
-   Stored in models/chunk_embeddings.npy

### 5️⃣ Sentiment Probability Modeling

Each chunk classified into:

-   Positive
-   Neutral
-   Negative

Probability distributions saved as sentiment_probs_semantic.npy
Chunk-level results stored in df_semantic_with_sentiment.csv

### 6️⃣ Aggregation Pipeline

  Level               Output File
  ------------------- ---------------------------------
  Chunk-level         df_semantic_with_sentiment.csv
  Review-level mean   review_level_sentiment_mean.csv
  Topic-level         final_semantic_sentiment.csv

### 7️⃣ Advanced Analysis

-   Factor Analysis (Dimensionality Reduction)\
-   Hierarchical Clustering\
-   Dendrogram construction\
-   Bank cluster visualization\
-   SWOT-style strategic interpretation

------------------------------------------------------------------------

## 📊 Analytical Capabilities

✔ Compare banks across semantic themes\
✔ Identify strengths and weaknesses per topic\
✔ Detect cluster-based similarity among banks\
✔ Visualize positioning using factor biplots\
✔ Construct strategy-oriented insights

------------------------------------------------------------------------

## 🚀 How to Run

1.  Clone the repository
    ```git clone git@github.com:sanjyay/bank-sentiment-analysis.git```

3.  Install dependencies using:

    ```pip install -r requirements.txt```

4.  Open notebooks/nlp.ipynb

------------------------------------------------------------------------

## 🧠 Tech Stack

-   Python
-   Pandas
-   NumPy
-   Scikit-learn
-   NLP Embedding Model
-   Sentiment Classification Model
-   Matplotlib
-   Seaborn

------------------------------------------------------------------------

## ⚠️ Disclaimer

-   Data is used strictly for academic and research purposes.\
-   This project has no affiliation with MouthShut.com or the banks
    analyzed.

