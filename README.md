User-Based Recommender System

📌 Introduction

The User-Based Recommender System is a product recommendation model based on user preferences. This project utilizes Singular Value Decomposition (SVD) to decompose the rating matrix, identify users with similar interests, and provide personalized recommendations.

📚 Technologies Used

🐍 Python (NumPy, Pandas, Scikit-learn)

📊 Machine Learning (SVD, Collaborative Filtering)

🔢 Linear Algebra (Matrix Decomposition)


🔍 How It Works

1️⃣ Data Preprocessing

Convert raw data into a User-Item matrix.

Handle missing values and sparse data.

2️⃣ Matrix Decomposition with SVD

The rating matrix is decomposed into three components:


Select an appropriate k value to reduce dimensionality while retaining essential information.

3️⃣ Prediction and Recommendation

Use Cosine Similarity to find users with similar preferences.

Rank products based on ratings from similar users.


🏆 Results

Improved accuracy compared to traditional Collaborative Filtering.

Reduced noise and handled sparse data efficiently.

More relevant recommendations based on user preferences.

📌 References

SVD in Recommendation Systems - GeeksforGeeks

Machine Learning Mastery - Recommender Systems

🎯 Contribution & Contact

📧 Nguyen Trung Hieu - hieuanthonydisward@gmail.com

If you find this project helpful, please ⭐ the repository on GitHub! 😊

