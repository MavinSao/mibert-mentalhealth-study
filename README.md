# Enhancing Mental Health Detection in Crisis-Related Social Media: A Domain-Adaptive Transformer Approach

## Description

This project focuses on developing a BERT-based mental health domain-adaptive transformer (MIBERT) for mental health classification across 8 categories:
- ADHD
- Anxiety
- Bipolar Disorder
- Depression
- PTSD
- OCD
- BPD
- None (No mental health condition)

We compare our proposed MIBERT model with other domain-specific pretrained models:
- BioBERT
- ClinicalBERT
- MedBERT
- Standard BERT

Additionally, we benchmark against traditional baseline approaches:
- TF-IDF + Logistic Regression
- GloVe + LSTM

## Model Configuration

### Hyperparameters
- Maximum sequence length: 256 tokens
- Batch sizes tested: 8, 16, 32
- Learning rates tested: 1e-5, 2e-5, 3e-5

### Models Compared
1. **MIBERT** (proposed): Our domain-adaptive transformer for mental health
2. **BERT**: The original BERT base model
3. **BioBERT**: BERT pretrained on biomedical text
4. **ClinicalBERT**: BERT pretrained on clinical notes
5. **MedBERT**: BERT pretrained on medical literature

## Evaluation Metrics

Our models are evaluated using:
- Accuracy
- F1 Score
- Precision
- Recall

## Explainability Analysis

We utilize SHAP (SHapley Additive exPlanations) to:
- Identify feature importance
- Focus on significant words in sentences
- Provide interpretable insights into model decisions

## Behavior Testing

We perform stress testing on our models using:
- **Synonym Replacement**: Testing model robustness to vocabulary variations
- **Masking**: Evaluating model performance with missing information

## License

Mavin Sao @CopyRight 2025 [MIT](https://choosealicense.com/licenses/mit/)