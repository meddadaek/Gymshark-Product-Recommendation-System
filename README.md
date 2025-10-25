# 🦈 Gymshark Product Recommendation System

An intelligent **hybrid recommendation system** that suggests Gymshark products based on **text features**, **vendor data**, and **price attributes**.  
The project combines **deep learning embeddings (TensorFlow/Keras)** with **cosine similarity** to deliver personalized and accurate product recommendations.

---

## 🚀 Project Overview

This notebook builds a system that:
- Trains a **multi-input neural network** using product titles, vendors, and prices  
- Learns product embeddings for classification and similarity computation  
- Uses **cosine similarity** to find the most relevant Gymshark items  
- Evaluates model accuracy, top-K performance, and confusion metrics  

The final system can predict a product’s category and recommend top similar items based on learned representations.

---

## 🧠 Model Architecture

- **Text Input** → Embedding Layer → Global Average Pooling  
- **Vendor Input** → Vendor Embedding → Flatten  
- **Price Input** → Dense Layer  
- **Concatenated Features** → Dense Layers → Dropout → Output (Softmax)

This architecture learns to represent Gymshark items as dense vectors, making it possible to compute **cosine similarity** between products for recommendation.

---

## 📊 Evaluation Metrics

- **Accuracy** and **Loss** on test data  
- **Precision, Recall, F1-score** via `classification_report`  
- **Top-3 Accuracy** (useful for multi-class recommendation tasks)  
- **Confusion Matrix Visualization** using Seaborn  
- **Training Curves** for Loss and Accuracy  

---

## 🧩 Technologies Used

| Category | Libraries |
|-----------|------------|
| Deep Learning | TensorFlow, Keras |
| Data Handling | NumPy, Pandas |
| Evaluation | scikit-learn |
| Visualization | Matplotlib, Seaborn |

---

## 🗂️ Project Structure

├── gymshark.ipynb # Main notebook with training, evaluation, and recommendations
├── data/ # (Optional) Product dataset (title, vendor, price, etc.)
├── README.md # Project documentation
└── requirements.txt # Dependencies list

yaml
Copier le code

---

## ⚙️ Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/meddadaek/gymshark-recommendation-system.git
   cd gymshark-recommendation-system
Install dependencies:

bash
Copier le code
pip install -r requirements.txt
Run the notebook:

bash
Copier le code
jupyter notebook gymshark.ipynb
💡 Example Output
yaml
Copier le code
Product: Flex Leggings
Top Recommendations:
- Energy Seamless Leggings | Vendor: Gymshark | Price: 55
- Adapt Animal Seamless Leggings | Vendor: Gymshark | Price: 60
- Vital Seamless 2.0 Leggings | Vendor: Gymshark | Price: 50
🔮 Future Enhancements
Add user behavior data for collaborative filtering

Integrate image embeddings using CNNs for visual similarity

Deploy via Flask/Streamlit as an interactive web app

Use FAISS or Annoy for scalable similarity search

🧑‍💻 Author
Abdelkader (Doro Kanji)
📍 Computer Science Student | Machine Learning Enthusiast
📧 Instagram
⭐ If you like this project, don’t forget to star the repo!
