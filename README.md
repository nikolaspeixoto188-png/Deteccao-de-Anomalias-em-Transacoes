# Detecção de Anomalias em Transações em Python

Projeto do bootcamp Bradesco - Dados, Cibersegurança e GenAI da DIO.

## Objetivo
Detectar transações fraudulentas (0.172% dos dados) usando técnicas de detecção de anomalias.

## Etapas do Projeto
**1. Primeiros Passos:** EDA, tratamento de Amount/Time com StandardScaler e modelo baseline Isolation Forest (contamination=0.0017).

**2. Avaliação e Balanceamento:** Dataset altamente desbalanceado. Aplicado SMOTE para balanceamento e avaliado com Precision, Recall, F1-Score e ROC-AUC. Acurácia descartada.

**3. Modelos Avançados e Explicabilidade:** 
- Random Forest + SMOTE: ROC-AUC 0.96
- XGBoost com scale_pos_weight: ROC-AUC 0.98
- Explicabilidade com SHAP mostrando V14, V17 e V10 como features mais importantes.

## Dataset
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## Como Executar
pip install -r requirements.txt
jupyter notebook deteccao_anomalias.ipynb
