# -multimodal-sentiment-analysis
 Multimodal Sentiment Analysis using BERT + ResNet-50 on MELD dataset
# Multimodal Sentiment Analysis

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0-orange.svg)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow.svg)

A deep learning project combining text (BERT) and facial image (ResNet-50)
features to predict sentiment from dialogue utterances on the MELD dataset.

---

## Notebooks (added daily)

| Day | Notebook | Colab |
|-----|----------|-------|
| Day 1 | Data & EDA | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ravitiw0009/-multimodal-sentiment-analysis/blob/main/notebooks/Day1_Data_EDA.ipynb) |
| Day 2 | Text & Image Models | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ravitiw0009/-multimodal-sentiment-analysis/blob/main/notebooks/Day2_Text_Image_Models.ipynb) |
| Day 3 | Fusion Model | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ravitiw0009/-multimodal-sentiment-analysis/blob/main/notebooks/Day3_Fusion_Model.ipynb) |
| Day 4 | Evaluation & Demo | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ravitiw0009/-multimodal-sentiment-analysis/blob/main/notebooks/Day4_Evaluation_Demo.ipynb) |

> Notebooks are being added daily as the project progresses.

---

## Architecture
Text Input  → BERT → [CLS] 768-dim  ─┐
├→ Concat 2816-dim → FC(512) → FC(3) → Sentiment
Image Input → ResNet-50 → 2048-dim  ─┘
---

## Results (updated after training)

| Model | Accuracy | F1 Score |
|-------|----------|----------|
| Text only (BERT) | TBD | TBD |
| Image only (ResNet-50) | TBD | TBD |
| **Fusion (concat)** | **TBD** | **TBD** |

---

## Dataset

[MELD — Multimodal EmotionLines Dataset](https://affective-meld.github.io/)
- 13,000+ utterances from Friends TV show
- Labels: Positive / Neutral / Negative
- Modalities: Text transcripts + face image frames

---

## Setup

```bash
git clone https://github.com/Ravitiw0009/-multimodal-sentiment-analysis.git
cd -multimodal-sentiment-analysis
pip install -r requirements.txt
```

---

## Tech Stack

`PyTorch` `HuggingFace Transformers` `torchvision` `SHAP` `Gradio` `scikit-learn`

---

## Acknowledgements

- BERT: Devlin et al., Google AI, Apache 2.0 License
- ResNet-50: He et al., PyTorch Model Zoo, BSD License
- MELD Dataset: Poria et al., USC — Academic use only

---

## Author

Ravi | Ravitiw0009 | ML&DL Trainee
