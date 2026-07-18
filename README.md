# Resume–Job Matching using Deep Siamese Bi-LSTM

This project explores automatic resume–job matching using Deep Learning and Natural Language Processing (NLP). The objective is to predict whether a resume matches a job description by learning semantic representations rather than relying solely on keyword similarity.

Our implementation is **based on the paper _Matching Resumes to Jobs via Deep Siamese Network_ by Sachin Maheshwary and Vinod Misra (WWW Companion 2018)**. While the original paper proposes a Siamese CNN architecture, we extend this work by replacing the CNN encoder with a **Bidirectional LSTM** and evaluating the impact of an **attention mechanism**.

A custom dataset was created by combining public resume and job posting datasets, with labels automatically generated using TF-IDF cosine similarity.

## Models

- TF-IDF + Logistic Regression
- Siamese CNN
- Siamese CNN + Attention
- Siamese Bi-LSTM
- Siamese Bi-LSTM + Attention

## Results

The attention-based Siamese models achieved up to **85.4% accuracy**, demonstrating improved semantic matching between resumes and job descriptions compared with traditional lexical approaches.

**Reference**

Maheshwary, S., & Misra, V. (2018). *Matching Resumes to Jobs via Deep Siamese Network*. Companion Proceedings of The Web Conference (WWW 2018).
