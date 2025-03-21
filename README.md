# User-Based Recommender System

## 📌 Introduction
The **User-Based Recommender System** is a product recommendation model based on user preferences. This project utilizes **Singular Value Decomposition (SVD)** to decompose the rating matrix, identify users with similar interests, and provide personalized recommendations.

## 📚 Technologies Used
- 🐍 **Python** (NumPy, Pandas, Scikit-learn)
- 📊 **Machine Learning** (SVD, Collaborative Filtering)
- 🔢 **Linear Algebra** (Matrix Decomposition)

## 🏗 Project Structure
```
User-Based-Recommender-System/
│── data/                    # Dataset folder
│── src/                     # Source code
│   ├── preprocess.py        # Data preprocessing
│   ├── svd_recommender.py   # SVD algorithm implementation
│   ├── evaluate.py          # Model evaluation
│── notebooks/               # Jupyter Notebooks for data analysis
│── README.md                # Project documentation
```

## 🔍 How It Works
### 1️⃣ **Data Preprocessing**
- Convert raw data into a `User-Item` matrix.
- Handle missing values and sparse data.

### 2️⃣ **Matrix Decomposition with SVD**
- The rating matrix is decomposed into three components: 
  \[ A = U \times \Sigma \times V^T \]
- Select an appropriate `k` value to reduce dimensionality while retaining essential information.

### 3️⃣ **Prediction and Recommendation**
- Use **Cosine Similarity** to find users with similar preferences.
- Rank products based on ratings from similar users.

## 🚀 How to Run the Project
### 1️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 2️⃣ Run the Recommender Model
```bash
python src/svd_recommender.py
```

### 3️⃣ Check Recommendation Results
```bash
python src/evaluate.py
```

## 📊 Example
```python
import numpy as np
from svd_recommender import SVDRecommender

# Create a sample rating matrix
A = np.array([
    [5, 4, 0, 1],
    [4, 0, 0, 1],
    [1, 1, 0, 5],
    [0, 0, 5, 4],
    [0, 1, 5, 4]
])

recommender = SVDRecommender(k=2)
recommender.fit(A)
recommendations = recommender.recommend(user_id=2)
print(recommendations)
```

## 🏆 Results
- Improved accuracy compared to **traditional Collaborative Filtering**.
- Reduced noise and handled sparse data efficiently.
- More relevant recommendations based on user preferences.

## 📌 References
- [SVD in Recommendation Systems - GeeksforGeeks](https://www.geeksforgeeks.org/svd-in-recommendation-systems/)
- [Machine Learning Mastery - Recommender Systems](https://machinelearningmastery.com/using-singular-value-decomposition-to-build-a-recommender-system/)

## 🎯 Contribution & Contact
📧 **Nguyen Trung Hieu** - [hieuanthonydisward@gmail.com](mailto:hieuanthonydisward@gmail.com)

If you find this project helpful, please ⭐ the repository on GitHub! 😊

