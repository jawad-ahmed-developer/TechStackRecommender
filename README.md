# Tech Stack Recommender

A content-based recommendation engine that maps a user's skills to the most relevant tech career paths using **TF-IDF Vectorization** and **Cosine Similarity**.

---

## 🚀 Overview

Tech Stack Recommender takes a list of user skills as input and returns the **Top 3 most relevant job roles** from a curated dataset.

Instead of relying on pretrained models or black-box algorithms, the system uses mathematical similarity measures to provide transparent and explainable recommendations.

---

## ⚙️ How It Works

```text
User Skills → TF-IDF Vectors → Cosine Similarity → Top 3 Roles
```

* **Dataset** — `raw_skills.csv` contains 20 technology roles and their associated skills.
* **IDF Calculation** — Rare skills receive higher importance than commonly occurring skills.
* **Vectorization** — User skills and job roles are represented in the same skill-vector space using TF-IDF.
* **Similarity Scoring** — Cosine Similarity is computed between the user vector and each role vector.
* **Ranking** — The Top 3 most relevant roles are returned.

---

## 🗂️ Project Structure

```text
tech-stack-recommender/
│
├── raw_skills.csv               # Dataset
├── tech_stack_recommender.ipynb # Main notebook
└── README.md
```

---

## 📦 Dependencies

```python
pandas
numpy
math
```

No external machine learning libraries are required.

---

## ▶️ Usage

```python
# Define your skills
inputs = ['AWS', 'Docker', 'Kubernetes']

# Run the notebook to generate recommendations
```

### Sample Output

```text
============================================================
Following are the recommended Roles based on the user input
============================================================

User Inputs: ['AWS', 'Docker', 'Kubernetes']

Recommended Roles:

#1 DevOps Engineer
Score  : 0.6823

#2 Cloud Engineer
Score  : 0.5341

#3 Site Reliability Engineer
Score  : 0.4102
```

---

## 📸 Screenshots

| Notebook Overview | Sample Output    |
| ----------------- | ---------------- |
| screenshot_1.png  | screenshot_2.png |

---

## 🧠 Concepts Applied

* TF-IDF (Term Frequency – Inverse Document Frequency)
* Cosine Similarity
* Vector Space Model
* Content-Based Filtering

---

## 👤 Author

**Jawad Ahmed**
BS Computer Science

Built as part of a Data Science / Machine Learning coursework project.
