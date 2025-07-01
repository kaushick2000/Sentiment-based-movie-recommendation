🎬 Sentiment-Based Movie Recommendation System
📌 Introduction
This project presents a sentiment-based movie recommendation system that utilizes a hybrid deep learning approach combining BERT embeddings and a CNN-BiLSTM architecture. The goal is to enhance recommendation accuracy by understanding the underlying sentiment in critic-style reviews, going beyond traditional collaborative filtering or content-based systems.

Unlike standard approaches that rely on user ratings or item similarity, this system interprets formal, analytical movie reviews to capture deeper sentiment cues and align them with user preferences.

The latest version of the system includes several major upgrades:

Advanced text preprocessing techniques

Revised model architecture

Integration with Gemini 1.5-pro, which enables transformation of unstructured queries into structured review-form inputs.

These enhancements help in better sentiment classification and more refined movie recommendations. The project also includes a detailed comparison between older and newer model versions, highlighting the evolution in design and performance.

📂 Dataset Description
The dataset used consists of critic-type movie reviews with a formal, structured tone. These reviews offer a rich source of sentiment information compared to casual user comments. Key components of the dataset include:

Movie Title

Review Text

Sentiment Labels (e.g., Fresh, Rotten)

Review Date

Movie Metadata (e.g., genre, release year)

🧹 Preprocessing
Version	Preprocessing Approach
Review 3	- Lemmatization
- Stop word removal
Review 4	- Full-text preserved for contextual richness

Tokenization was performed on each review.

BERT embeddings were generated to capture high-level semantic information.

These embeddings were passed through a CNN-BiLSTM hybrid model.

To address class imbalance, class_weight='balanced' was applied during CNN training.

This comprehensive approach allows the model to learn complex sentiment patterns and deliver more context-aware, sentiment-driven movie recommendations.

🚀 Key Technologies
 BERT (Bidirectional Encoder Representations from Transformers)

 CNN-BiLSTM Hybrid Model

 Gemini 1.5-pro for query structuring

 Python / TensorFlow / PyTorch (depending on implementation)

 NLP Preprocessing Techniques (tokenization, lemmatization, etc.)

📈 Outcomes
Improved sentiment classification accuracy

More personalized and context-rich recommendations

Enhanced understanding of structured vs. unstructured input handling
