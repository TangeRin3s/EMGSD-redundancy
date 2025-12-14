## 1. Baseline Replication

To ensure methodological rigor, I fully replicated the baseline stereotype classification pipeline from the HEARTS framework.

### 1.1 Repository Cloning

I successfully cloned and executed the official HEARTS repository:

git clone https://github.com/holistic-ai/HEARTS-Text-Stereotype-Detection

All scripts executed without modification after environment reconstruction.

## 2. Environment & Dependency Documentation

Requirements.txt and environment.yml are provided.

## 3. Reproducing Baseline Results

To validate replication quality, I re-trained the baseline ALBERT-V2 stereotype classifier on the original EMGSD dataset. Besides, To show small-scale training works, I train a
ALBERT-V2 model and a xlm-roberta-base model in a small dataset with only 5000 samples.

### My results vs Original results (Evaluate on EMGSD)

| Metric    | Original (Paper) | ALBERT-V2 | XLM-RoBERTa-base |
|-----------|------------------|-----------|------------------|
| Macro-F1  | 81.5%            | 82%       | 82%              |





