# GenreGenius: Hybrid Music Recommendation System  


A hybrid music recommender system blending **collaborative filtering** (user patterns) and **content-based filtering** (audio features) to tackle the cold-start problem. Built for the *Applied AI* coursework at the University of Westminster.  

## 🎯 Key Features  
- **Hybrid Model**: Combines Matrix Factorization (MF) predictions with audio feature similarity.  
- **Cold-Start Handling**: Recommends new tracks/users using content analysis when interaction data is sparse.  
- **Scalable**: Built with Python, Surprise, and TensorFlow.  

## 📦 Datasets  
1. **Kaggle Million Song Dataset**: 50k+ tracks with audio features.  
2. **Personal Spotify Streaming History**: Real-world user listening logs.  

## 🛠️ System Architecture  
1. **Data Integration**: Merge Kaggle and Spotify data.  
2. **Preprocessing**: Filtering, log-transform playcounts, scaling features.  
3. **Models**:  
   - **Matrix Factorization (MF)**: Predict user-song affinity.  
   - **Autoencoder (Optional)**: Deep learning-based exploration.  
   - **Hybrid Engine**: Weighted fusion of CF and content scores.  

## 📊 Results  
| Metric          | Score       |
|-----------------|-------------|
| RMSE (MF)       | 0.49        |
| Recall@10 (MF)  | 1.0         |

## 🚀 Getting Started  
### Dependencies  
- Python 3.8+  
- Libraries: `pandas`, `numpy`, `surprise`, `tensorflow`, `scikit-learn`  

### Installation  
```bash
git clone https://github.com/yourusername/GenreGenius.git
pip install -r requirements.txt
