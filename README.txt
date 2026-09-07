U-CARE V12 FINAL RESEARCH PACKAGE
=================================

Project:
U-CARE: Uncertainty-Aware Cross-Modal Attention Network
with Explainable AI for Retinal Disease Analysis

Model:
U-CARE V12

Modalities:
1. Fundus
2. OCT

Architecture:
- EfficientNet-B0 Fundus Encoder
- EfficientNet-B0 OCT Encoder
- Cross-Modal Attention Fusion
- Binary Disease Classifier
- Monte Carlo Dropout Uncertainty
- Grad-CAM Explainability

Patient-level split:
Train: 83 patients
Validation: 18 patients
Test: 18 patients

Patient leakage:
ZERO

Final test cohort:
18 patients
34 multimodal records

Final threshold:
0.33

Final test metrics:
Accuracy: 88.89%
Precision: 100.00%
Sensitivity/Recall: 50.00%
Specificity: 100.00%
F1-score: 66.67%
Balanced Accuracy: 75.00%
ROC-AUC: 100.00%
PR-AUC: 100.00%

Important research limitation:
The current V12 dataset does not contain genuine clinical
variables or longitudinal follow-up/progression labels.
Therefore personalized clinical prediction and progression
risk prediction are NOT claimed as experimentally validated
components of the current V12 results.

The included uncertainty and Grad-CAM experiments are
experimental explainability/uncertainty components.

Use the V12 model checkpoint for the existing Streamlit
frontend after updating the model path.