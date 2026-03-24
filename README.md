# Thonburian-Whisper-Khummuang

A Jupyter Notebook project for fine-tuning **Thonburian Whisper** on the **Khummuang dialect** (Northern Thai).

## Project Overview

This project focuses on adapting a pretrained Whisper-based model to better understand **Khummuang**, a northern dialect of Thai. To improve performance in this low-resource setting, we incorporate:

- **Pseudo-labeling** to expand the effective training data  
- **Data filtering** to improve label quality and reduce noise  

These techniques help enhance model robustness and transcription accuracy for dialectal speech.

📘 The full fine-tuning tutorial is available in the Jupyter Notebook:  
`finetune_thonburian_whisper.ipynb`

---
## Training Dataset
We use the Khummuang dataset from the thai-dialect-corpus dataset [Link]( https://github.com/SLSCU/thai-dialect-corpus).

The structure of data for training and testing should be in this structure for the notebook

### Expected Data Structure
```
khummuang/
├── audio/
│   ├── dev_audio00/
│   └── train_audio00/
├── dev.csv
└── train.csv
```

- `audio/` — Contains all audio files  
  - `train_audio00/` — Training audio samples  
  - `dev_audio00/` — Validation (development) audio samples  
- `train.csv` — Metadata and transcripts for training data  
- `dev.csv` — Metadata and transcripts for validation data  
