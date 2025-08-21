# LeGalFormer: Legal Judgment Prediction using Graph-Enhanced Transformers

## Overview
Implementation of LeGalFormer for Legal Judgment Prediction, extending the model from legal case retrieval to court outcome prediction.

## Key Results
- **Accuracy:** 91.80%
- **Macro-F1:** 87.73% 
- **Parameters:** 3.2M (97% reduction vs traditional transformers)
- **Dataset:** ECtHR (European Court of Human Rights)

## Description
This repository contains the implementation for my MSc thesis at University of Galway. The model converts legal cases into Legal Case Element Graphs (LCEGs) and uses graph-enhanced transformers with three encoding mechanisms:
- Centrality encoding for node importance
- Edge encoding for relationship semantics
- Spatial encoding for structural distance

## Performance Comparison
| Method | Accuracy | Macro-F1 | Parameters |
|--------|----------|-----------|------------|
| BERT | 90.50% | 85.96% | 110M |
| BERT+Att+GCN | 91.60% | 86.87% | 120M |
| **LeGalFormer** | **91.80%** | **87.73%** | **3.2M** |

## Citation
```bibtex
@mastersthesis{muruganantham2025,
    title={Legal Judgement Prediction using LeGalFormer: A Graph Enhanced Transformer Approach},
    author={Muruganantham, Mukhunth},
    year={2025},
    school={University of Galway}
}
