<img width="768" height="458" alt="image" src="https://github.com/user-attachments/assets/1a8a056f-96ae-4af2-b631-918be776a056" />Tech Stack Recommender

A content-based recommendation engine that maps a user's skills to the most relevant tech career paths using TF-IDF vectorization and Cosine Similarity.


🚀 Overview
Tech Stack Recommender takes a list of user skills as input and returns the Top 3 most relevant job roles from a curated dataset. It transforms qualitative career guidance into objective, ranked mathematical output — no black box, no pretrained model.

⚙️ How It Works
User Skills → TF-IDF Vectors → Cosine Similarity → Top 3 Roles

Dataset — raw_skills.csv stores 20 job roles, each with an associated skill set
IDF — Computed across all roles to weight rare skills higher
Vectorization — Every role and the user input are mapped into the same n_skills dimensional vector space using TF-IDF
Scoring — Cosine similarity is calculated between the input vector and every role vector
Output — Top 3 roles ranked by similarity score


🗂️ Project Structure
tech-stack-recommender/
│
├── raw_skills.csv               # Dataset — 20 roles with skills
├── tech_stack_recommender.ipynb # Main notebook
├── tech_stack_recommender.py # Main notebook
└── README.md

📦 Dependencies
python
pandas
numpy
math   # standard library
No external ML libraries required.

▶️ Usage & 📸 Screenshots
# Run the notebook — output prints Top 3 recommended roles
# input1 = ['AWS', 'Docker', 'Kubernetes']
<img width="710" height="458" alt="image" src="https://github.com/user-attachments/assets/3ce70f17-77ab-4954-b8c3-f5a6c4b10a6f" />


# input2 = ['TensorFlow', 'PyTorch', 'Deep Learning']

<img width="865" height="459" alt="image" src="https://github.com/user-attachments/assets/e5c06b2b-a5e1-41f1-9b77-a970b862263a" />


# input3 = ['Java', 'Spring Boot', 'Microservices']

<img width="768" height="458" alt="image" src="https://github.com/user-attachments/assets/b51f7d65-4f16-47d9-8026-3b5cef491836" />

🧠 Concepts Applied

Term Frequency — Inverse Document Frequency (TF-IDF)
Cosine Similarity
Vector Space Model
Content-Based Filtering


👤 Author
Jawad Ahmed — BS Computer Science

Built as part of ML Internship at Decodelab 
