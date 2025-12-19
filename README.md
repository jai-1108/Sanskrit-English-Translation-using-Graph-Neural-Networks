# 🕉️ Sanskrit → English Translation using Graph Neural Networks (GNN)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red.svg)
![GNN](https://img.shields.io/badge/Graph%20Neural%20Networks-NLP-green.svg)
![NLP](https://img.shields.io/badge/NLP-Machine%20Translation-purple.svg)
![IEEE](https://img.shields.io/badge/IEEE-Accepted%20Publication-blue.svg)

📄 **Accepted at IEEE ICCCSMD 2024**

---

## 📌 Overview

This project explores **Graph Neural Networks (GNNs)** for **Sanskrit-to-English machine translation**, addressing challenges posed by Sanskrit’s highly inflectional grammar and flexible word order.  
Instead of treating sentences as sequences, we model them as **graphs**, allowing the model to capture **syntactic and semantic dependencies** more effectively.

---

## 🚀 Key Contributions

- Modeled Sanskrit sentences as **dependency graphs** to better represent grammatical structure  
- Implemented **Graph Convolutional Networks (GCNs)** for syntax-aware translation  
- Achieved **BLEU score of 0.81**, outperforming traditional RBMT+DMT, RNN, and LSTM baselines  
- Demonstrated improved **fluency (3.82/4)** and **adequacy (3.85/4)** via human evaluation  

---

## 🧠 Methodology

### Graph Construction
- **Nodes**: Sanskrit tokens (words)  
- **Edges**: Syntactic dependencies derived from dependency parsing  

Each sentence is represented as a graph, enabling the model to capture both **local and global grammatical relationships**.

### Model Architecture
- Pre-trained word embeddings for node features  
- Two-layer **Graph Convolutional Network (GCN)**  
- Mean pooling to generate sentence embeddings  
- Fully connected + softmax layer for translation prediction  

---

## 📊 Results

| Model | BLEU Score |
|------|-----------|
| RBMT + DMT | 0.7606 |
| RNN | 0.72 |
| **GNN (Ours)** | **0.81** |

Additional improvements:
- ↓ Word-order errors by **~10%**
- ↓ Semantic errors by **~11%**
- Highest fluency and adequacy scores across models

---

## 🛠 Tech Stack

- **Language**: Python  
- **Deep Learning**: PyTorch  
- **NLP**: NLTK  
- **Models**: Graph Neural Networks (GCN)  
- **Evaluation**: BLEU, Accuracy, Human Fluency & Adequacy Scores  

---

## 📚 Dataset

- ~93,000 Sanskrit shlokas with English translations  
- Sources include **Ramayana** and **Mahabharata**  
- Split into training, validation, and test sets  

---

## 📄 Publication

> *Enhancing Sanskrit-to-English Translation Through Graph Neural Networks*  
Accepted at **IEEE ICCCSMD 2024**

---

## 🔮 Future Work

- Integrating **Transformer attention mechanisms** with GNNs  
- Extending approach to other **low-resource or ancient languages**  
- Scaling to larger multilingual corpora  

---

## 👤 Author

**Jai Vasi**  
MS Data Science, Stony Brook University  
📧 jai.n.vasi1108@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/jaivasi1108) | [GitHub](https://github.com/jai-1108)

---
