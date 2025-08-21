# LeGalFormer: Legal Judgment Prediction using Graph-Enhanced Transformers

## 📋 Overview

This repository contains the implementation of LeGalFormer for Legal Judgment Prediction, extending the original LeGalFormer model from legal case retrieval to court outcome prediction. The model achieves state-of-the-art performance on the European Court of Human Rights (ECtHR) dataset.

## 🏆 Key Results

- **Accuracy:** 91.80%
- **Macro-F1:** 87.73%
- **Parameters:** 3.2M (97% reduction vs traditional transformers)
- **Inference Time:** 45ms (50% faster than baselines)

## 🚀 Features

- **Graph-Enhanced Architecture:** Converts legal cases into Legal Case Element Graphs (LCEGs)
- **Triple Encoding System:**
  - Centrality encoding for node importance
  - Edge encoding for relationship semantics  
  - Spatial encoding for structural distance
- **Contrastive Learning:** Enhanced representation learning with similar/dissimilar case pairs
- **Efficient Design:** Dramatically reduced computational requirements

## 📊 Performance Comparison

| Method | Accuracy | Macro-F1 | Parameters | Inference Time |
|--------|----------|-----------|------------|----------------|
| BERT | 90.50% | 85.96% | 110M | 89ms |
| RoBERTa | 90.60% | 85.98% | 110M | 91ms |
| BERT+Att+GCN | 91.60% | 86.87% | 120M | 134ms |
| **LeGalFormer** | **91.80%** | **87.73%** | **3.2M** | **45ms** |

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/legalformer-legal-judgment-prediction.git
cd legalformer-legal-judgment-prediction

# Install dependencies
pip install -r requirements.txt

# Download required datasets
python download_data.py
