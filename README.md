# Thonburian-whisper-khummuang
A Jupyter Notebook for Fine-Tuning Thonburian Whisper on the Khummuang Dialect

## Training Dataset
We use the Khummuang dataset from the thai-dialect-corpus dataset [Link]( https://github.com/SLSCU/thai-dialect-corpus).

The structure of data for training and testing should be in this structure for the notebook

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
