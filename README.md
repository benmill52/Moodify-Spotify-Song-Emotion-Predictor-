# 🎵 Moodify – Spotify Song Emotion Predictor  

Moodify is a machine learning–powered music emotion classification system built as part of the **Poshem Tech 30 Days Data Challenge**.

The project predicts the emotional category of songs using Spotify audio features and transforms those predictions into meaningful user insights through an interactive web application.

---

## 🚀 Project Overview  

Moodify classifies songs into four emotional categories:

- 🎭 **Sad**  
- 😊 **Happy**  
- ⚡ **Energetic**  
- 🌿 **Calm**

The system uses structured Spotify audio features such as:

- Danceability  
- Energy  
- Loudness  
- Valence  
- Acousticness  
- Tempo  

### 🎯 Objective  

To build a robust multi-class classification model capable of accurately predicting the emotional tone of a track and demonstrate how data-driven insights can power music recommendation systems.

---

## 🧠 Problem Statement  

Music streaming platforms rely heavily on personalization. However, categorizing songs by emotion manually is subjective and not scalable.

This project explores:

- Can we predict a song’s emotional category using only audio features?
- Which machine learning algorithm performs best for this structured classification task?
- How can we deploy the model into a usable product?

---

## 🛠️ Tech Stack  

- **Python**
- **Pandas / NumPy**
- **Scikit-learn**
- **LightGBM**
- **Matplotlib / Seaborn**
- **Streamlit**

---

## 📊 Exploratory Data Analysis (EDA)  

Key steps included:

- Distribution analysis of audio features  
- Outlier inspection  
- Feature-target relationship exploration  
- Correlation analysis  
- Class imbalance assessment  

This ensured a solid understanding of the dataset before modeling.

---

## 🤖 Models Explored  

To identify the best-performing algorithm, the following models were trained and evaluated:

- Decision Tree  
- Random Forest  
- Logistic Regression  
- LightGBM  

### 🏆 Final Model: LightGBM  

LightGBM delivered the most consistent and strongest performance across evaluation metrics, particularly in handling non-linear feature interactions.

---

## 📈 Model Evaluation  

To ensure reliable performance and prevent overfitting:

- ✅ **10-Fold Cross-Validation**
- 🎯 **Primary Metric: F1-Weighted Score**
- 📌 Additional Metrics:
  - Accuracy  
  - Precision  
  - Recall  
  - Confusion Matrix  

### Why F1-Weighted?  

Because this is a multi-class problem with potential class imbalance, the weighted F1 score ensures fair evaluation across all emotional categories instead of favoring dominant classes.

---

## 🌐 Deployment  

The trained LightGBM model was deployed using **Streamlit**, creating an interactive web application where users can:

- Input song audio features  
- Receive predicted emotional category  
- Generate music personality insights  
- (Optional) Integrate LLM-powered explanations  

This demonstrates the complete machine learning lifecycle:

> Data → Modeling → Evaluation → Deployment → User Interaction
