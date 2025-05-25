# 📊 Hierarchical Clustering on Job Listings

This project performs hierarchical clustering on job listings scraped from a job portal. It groups jobs based on the required skills, allowing users to explore similar roles interactively via a Streamlit web app.

---

## 📁 Project Structure


---

## 📌 Overview

The goal of this project is to help users explore job listings grouped by similarity in skill requirements. Using **Hierarchical Clustering**, similar jobs are grouped into clusters without any prior labeling.

A user-friendly Streamlit app allows filtering and exploring jobs by cluster.

---

## 🔍 Data Collected

Each job listing contains the following fields:

- **Job Title**
- **Company Name**
- **Location**
- **Skills** (used for clustering)

Data was scraped from Karkidi.com using `BeautifulSoup` and stored in a structured format.

---

## 🧹 Preprocessing Steps

1. **Clean text**: Remove punctuation, convert to lowercase.
2. **Tokenize** skills into separate terms.
3. **TF-IDF Vectorization**: Transform skills into numerical vectors using `TfidfVectorizer`.

---

## 🧠 Clustering Method

- **Technique**: Agglomerative **Hierarchical Clustering**
- **Tool**: `scipy.cluster.hierarchy` and `sklearn`
- **Dendrogram**: Used to determine the optimal number of clusters by visual inspection.
- Jobs are grouped into clusters based on TF-IDF similarity of skills.

---

## 📈 Evaluation

Clusters were evaluated **manually** by inspecting job titles and dominant skills in each group. For example, clusters dominated by "Python", "SQL", and "Machine Learning" clearly represent data-related roles.

---

## 🌐 Streamlit App

Run the app to explore jobs by cluster.

### 💻 Features:
- View all job listings in a table
- Filter jobs by one or more cluster numbers
- Simple and interactive UI

---

## 🚀 How to Run the Project

### 1. Clone the repository:
```bash
git clone https://github.com/anshif20022kt/Hierarchical-clustering.git
cd Hierarchical-clustering
pip install -r requirements.txt
streamlit run app.py

---
📚 Technologies Used

Python
BeautifulSoup
Pandas, NumPy
Scikit-learn
Streamlit
TF-IDF Vectorization
Hierarchical Clustering
📬 Contact

Developed by Anshif KT
For questions or collaboration, feel free to open an issue or contact via GitHub.

Let me know if you'd like a version with badges, contribution guidelines, or deployment steps for Streamlit Cloud or Hugging Face Spaces.
