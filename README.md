# A project for UCL Course COMP0173 AI for sustainable development.

Aiming to show the redundancy of EMGSD dataset and the feasibility of small-scale training models and multi-linguistic models.

Original paper: HEARTS: A Holistic Framework for Explainable, Sustainable and Robust Text Stereotype Detection - https://arxiv.org/abs/2409.11579

Original github repository: https://github.com/holistic-ai/HEARTS-Text-Stereotype-Detection

## Relation to SDGs

• **SDG 12 – Responsible Consumption & Production:**  
Lower energy use and model carbon footprints, supporting AI development aligned with sustainable consumption of digital resources.

• **SDG 9 – Industry, Innovation & Infrastructure:**  
Reduce costs, making models accessible to low-resource institutions and supporting equitable AI innovation.

• **SDG 10 – Reduced Inequalities:**  
Enable stereotype detection across groups and languages, helping mitigate social and linguistic inequalities.




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

Here are two illustrations of model performances.
<img width="1028" height="724" alt="image" src="https://github.com/user-attachments/assets/ccd61d0c-5401-4f32-8668-c638c75d2ee3" />
<img width="922" height="657" alt="image" src="https://github.com/user-attachments/assets/53a51c57-20c4-4fa6-a407-8b7e68e9a4ce" />

## 4. Reproducible Code & Notebooks

To ensure experimental reproducibility, all experiments were conducted with a fixed random seed:

- **Random seed:** 42

Here are introductions for important files.<br>

1, BERT_Models_Fine_Tuning.ipynb<br>

Where ALBERT-V2 models and xlm-roberta-base models are trained.<br>

2, Translate.ipynb<br>

Show How to use Chatgpt to translate a sampled dataset from MGSD to Chinese and Japanese.<br>

3, redundancy.ipynb<br>

Ploting illustrations to show the redundancy fo EMGSD.<br>

4, SHAP_LIME_Analysis.py<br>

Conducting Shap and Lime analysis of model.<br>






