# Spotify Data Analysis and Classification

This project applies supervised and unsupervised machine learning to Spotify track data to analyze patterns in music and predict both **track popularity** and **genre**.

## Project Goals
- Predict whether a song is **high** or **low** popularity
- Classify songs into grouped **genre categories**
- Use **PCA** and **K-Means** to explore patterns in the dataset

## Dataset
- 230,000+ Spotify tracks
- Audio features such as danceability, energy, loudness, speechiness, acousticness, tempo, and valence
- Data was cleaned, scaled, and transformed before modeling

## Models Used
- Decision Tree
- Random Forest
- Gradient Boosting / XGBoost
- Neural Network
- PCA
- K-Means Clustering

## Results
- For **popularity classification**, **Random Forest** gave the best accuracy at **71%**, while **XGBoost** was much faster with competitive performance at **69%**.
- For **genre classification**, **XGBoost** reached **64% accuracy** in only **4 seconds**.
- The best **Neural Network** model slightly outperformed tree-based genre models with **64.68% accuracy** and the highest precision.

### Key Takeaways
- **Model 3** performed best overall among neural networks
- **XGBoost** was the fastest strong baseline for genre classification
- Neural networks handled imbalance better when trained on downsampled data

## Key Findings
- Audio features can meaningfully predict both **song popularity** and **genre**
- **Acousticness**, **speechiness**, and related features were influential in popularity prediction
- For genre prediction, models performed better on some classes than others, especially when class balance improved
- **XGBoost** offered the best speed-to-performance tradeoff
- **Neural Network Model 3** delivered the strongest overall genre classification performance.
  
## Conclusion
The project shows that Spotify audio features can be used effectively for both classification and clustering. Tree-based models worked well for speed and interpretability, while neural networks gave the strongest overall genre prediction performance.
