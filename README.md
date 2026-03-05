# Comment Toxicity Classification using BERT and Graph Neural Networks (GNN)

A deep learning pipeline for detecting toxic comments on social media using **BERT for semantic understanding** and **Graph Neural Networks (GNN) for relational learning**.

This project combines **transformer-based language modeling** with **graph-based learning** to improve classification of toxic comments in online discussions.

---

## 📌 Project Overview

Online platforms increasingly face the challenge of moderating harmful content. Toxic comments can damage online communities and negatively affect users.

This project proposes a **hybrid deep learning architecture combining BERT and Graph Neural Networks** to accurately detect and classify toxic comments.

The system:

1. Extracts **semantic representations using BERT**
2. Builds a **graph structure of comments**
3. Applies **Graph Convolutional Networks (GCN)** to capture relationships between comments
4. Produces a **toxicity score between 0 and 1** for each comment 

---

## 🧠 Model Architecture

The architecture consists of two primary components:

### 1️⃣ BERT (Bidirectional Encoder Representations from Transformers)

BERT processes comment text and extracts contextual embeddings using:

- Tokenization
- Padding and truncation
- Word embeddings
- Positional embeddings
- Self-attention layers
- Feed-forward neural networks 

BERT generates semantic embeddings that represent the meaning of each comment.

---

### 2️⃣ Graph Neural Network (GNN)

The extracted embeddings are passed to a Graph Neural Network where:

- Each **node represents a comment**
- **Edges represent semantic similarity between comments**
- Graph convolution layers aggregate contextual information
- Hierarchical pooling summarizes the graph representation 

The GNN learns relationships between comments and improves classification performance.

---


---

## ⚙️ Methodology

### Data Preprocessing

The pipeline performs:

- Tokenization
- Special tokens `[CLS]` and `[SEP]`
- Padding and truncation
- Word embeddings
- Positional embeddings 

---

### Self Attention

BERT uses self-attention to understand relationships between words in a sentence.

Each token generates:

- Query vectors
- Key vectors
- Value vectors

These vectors compute contextual attention scores across the sequence.

---

### Classification Layer

The final BERT representation is passed through:

- Fully connected layers
- Softmax activation

The output produces a **toxicity probability score between 0 and 1**.

---


This allows the model to learn **relationships between semantically similar comments**.

---

## 📊 Evaluation Metrics

The model was evaluated using standard classification metrics:

- Accuracy
- Precision
- Recall
- F1 Score 

Example training results show consistent performance improvements across epochs.

---

## 📈 Results

The model demonstrates effective toxic comment detection using the combined architecture.

Typical results include:

| Metric | Value |
|------|------|
| Validation Accuracy | ~0.92 |
| Precision | ~0.41 |
| Recall | ~0.92 |
| F1 Score | ~0.91 |

---

## 🧪 Statistical Validation

A **t-test** was conducted on the recall metric to evaluate statistical significance of the results.

The t-test confirms that the model improvements are statistically meaningful. 

---


---

## 🛠 Technologies Used

- Python
- PyTorch
- HuggingFace Transformers
- Graph Neural Networks
- NLP
- Deep Learning

---

## 📚 Dataset

The model was trained using the **Jigsaw Unintended Bias in Toxicity Classification dataset**, which contains labeled comments with multiple toxicity categories. 

---

## 🚀 Future Improvements

Possible improvements include:

- Graph Attention Networks (GAT)
- Larger transformer models
- Bias mitigation techniques
- Multi-label classification improvements
- Real-time moderation API

---

## 👨‍💻 Authors

- Pavan Teja Reddy Kallam
- Susmitha Dudipalli
- Sukanya Karasala
- **Romith Bondada**

SRM University – AP  
Bachelor of Technology in Computer Science and Engineering

---

## 📄 License

This project is intended for **academic and research purposes**.

