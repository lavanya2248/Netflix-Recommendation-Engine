# 🎬 Personalized Streaming Recommendation Engine

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikitlearn)
![Surprise](https://img.shields.io/badge/Surprise-Recommendation%20System-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![License](https://img.shields.io/badge/License-MIT-green)

A machine learning-powered movie recommendation system that combines **Popularity-Based Filtering**, **Content-Based Filtering**, and **Collaborative Filtering (SVD)** to deliver personalized movie recommendations. Built using over **1 million user ratings**, the project demonstrates how modern streaming platforms can improve user engagement through intelligent recommendation algorithms.

---

# 📌 Project Overview

Recommendation systems play a crucial role in modern OTT streaming platforms by helping users discover relevant content while improving customer engagement and retention.

This project develops a complete recommendation engine capable of:

- Handling new users with no watch history
- Recommending similar movies using content similarity
- Generating personalized recommendations using Collaborative Filtering
- Addressing the sparsity problem commonly found in real-world recommendation systems

The solution was developed as part of the **Intellipaat Data Science & Analytics Capstone Project**.

---

# 🎯 Business Problem

Streaming platforms contain thousands of movies, making content discovery increasingly difficult for users.

Traditional popularity-based recommendations often:

- Recommend the same blockbuster movies
- Ignore niche but highly rated content
- Fail to personalize recommendations
- Reduce long-term user engagement

The objective of this project is to build a recommendation engine capable of understanding user preferences and recommending unseen movies likely to receive high ratings.

---

# 🎯 Objectives

- Analyze movie ratings and user behavior
- Identify the most popular and highest-rated genres
- Build multiple recommendation strategies
- Develop a personalized recommendation engine using Matrix Factorization (SVD)
- Evaluate recommendation performance using RMSE and MAE

---

# 📊 Dataset

The project utilizes the MovieLens dataset consisting of two primary datasets.

## movies.csv

Contains movie metadata including:

- Movie ID
- Movie Title
- Genres

**Total Movies:** 27,278

---

## ratings.csv

Contains user interaction data including:

- User ID
- Movie ID
- Rating
- Timestamp

**Total Ratings:** 1,048,575

---

# 📈 Dataset Statistics

| Metric | Value |
|---------|------:|
| Movies | 27,278 |
| Users | 7,120 |
| Rated Movies | 14,026 |
| Ratings | 1,048,575 |
| Matrix Sparsity | **98.95%** |

The high sparsity reflects a realistic recommendation system scenario where most users rate only a small fraction of the available movies.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Surprise Library
- TF-IDF Vectorizer
- Cosine Similarity
- Singular Value Decomposition (SVD)

---

# ⚙️ Data Preprocessing

The preprocessing pipeline includes:

- Extracting release year using Regular Expressions
- Cleaning movie titles
- Standardizing article placement (e.g., "Matrix, The" → "The Matrix")
- Formatting genre strings
- Converting Unix timestamps into readable datetime format

---

# 📊 Exploratory Data Analysis

The project explores:

- Rating distribution
- User activity distribution
- Most rated movies
- Highest-rated movies
- Genre popularity
- Average ratings by genre

### Key Insights

- Ratings are concentrated around 3–5 stars.
- User activity follows a long-tail distribution.
- Drama and Comedy receive the highest number of ratings.
- Film-Noir, Documentary, and War genres achieve the highest average ratings.

---

# 🧠 Recommendation System Architecture

The recommendation engine combines three complementary approaches.

## 1️⃣ Popularity-Based Recommendation

Designed for new users with no historical interaction.

Features:

- Minimum rating threshold
- Average rating ranking
- Cold-start solution

---

## 2️⃣ Content-Based Recommendation

Uses movie metadata to identify similar content.

### Techniques

- TF-IDF Vectorization
- Cosine Similarity

This enables recommendations based on genre similarity.

---

## 3️⃣ Collaborative Filtering (SVD)

The primary recommendation engine uses **Singular Value Decomposition (SVD)** to learn latent relationships between users and movies.

Instead of relying solely on genres, SVD discovers hidden user preferences through matrix factorization.

This approach effectively handles sparse user-item interactions and produces personalized recommendations.

---

# 📐 Model Evaluation

The model was trained using an **80/20 train-test split**.

## Evaluation Metrics

| Metric | Score |
|---------|-------|
| RMSE | **0.8334** |
| MAE | **0.6375** |

### Interpretation

- Low MAE indicates that predicted ratings are close to users' actual ratings.
- Similar RMSE and MAE values suggest stable model performance with limited extreme prediction errors.

---

# 🎥 Sample Recommendations

Example personalized recommendations generated for **User 1**:

| Movie | Predicted Rating |
|--------|-----------------:|
| Celebration (Festen) | 4.49 |
| The Lady Eve | 4.48 |
| Black Mirror | 4.46 |
| Stop Making Sense | 4.45 |
| Head-On (Gegen die Wand) | 4.44 |

---

# 📁 Project Structure

```
Netflix-Recommendation-Engine/
│
├── Netflix_Recommendation_Engine.ipynb
├── movies.csv
├── ratings.csv
├── Project_Report.txt
├── README.md
└── requirements.txt
```

---

# ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Netflix-Recommendation-Engine.git
```

Navigate into the project:

```bash
cd Netflix-Recommendation-Engine
```

Install dependencies:

```bash
pip install pandas numpy matplotlib scikit-learn scikit-surprise
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
Netflix_Recommendation_Engine.ipynb
```

---

# 🚀 Features

- Popularity-based recommendations
- Content-based movie recommendations
- Collaborative filtering using SVD
- Genre analysis
- User behavior analysis
- Recommendation prediction engine
- Recommendation evaluation metrics

---

# 📈 Business Impact

The recommendation engine helps streaming platforms:

- Improve user engagement
- Increase watch time
- Recommend niche high-quality content
- Reduce dependence on blockbuster recommendations
- Enhance user satisfaction through personalization

---

# 🔮 Future Improvements

- Hybrid recommendation systems
- Neural Collaborative Filtering (NCF)
- Deep Learning-based recommendation models
- Temporal recommendation modeling
- Real-time recommendation APIs
- Deployment using Streamlit or Flask

---

# 💡 Skills Demonstrated

- Machine Learning
- Recommendation Systems
- Data Cleaning
- Exploratory Data Analysis
- Matrix Factorization
- Collaborative Filtering
- Content-Based Filtering
- TF-IDF
- Cosine Similarity
- Model Evaluation
- Python Programming
- Data Visualization

---

# 👩‍💻 Author

**M. Lavanya**

📧 Email: lavanyalavu54321@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/lavanyalavu/

📱 Mobile: +91 9346481495

---

# 📄 License

This project is intended for educational and portfolio purposes. Feel free to use or modify it with proper attribution.

---

⭐ If you found this project useful, consider giving it a star on GitHub!