# KAIRI-SAFE Risk Measurement and Applications to Financial Model Risk Assessment

This repository contains a research paper on applying the KAIRI-SAFE framework to financial model risk assessment. The paper examines how AI model risks can be measured through the four SAFE dimensions: Sustainability, Accuracy, Fairness, and Explainability.

The paper proposes a structured approach for translating statistical model evaluation metrics into financial risk management indicators. It also introduces an aggregate SAFE rating that combines multiple AI risk indicators into a model-level assessment.

## Paper Overview

Artificial intelligence is increasingly used in financial services, including credit scoring, portfolio management, fraud detection, insurance underwriting, and risk forecasting. While AI models may improve predictive performance, they also introduce risks related to robustness, accuracy, fairness, and explainability.

This paper builds on and extend the KAIRI-SAFE framework proposed by Bracke et al. (2024) and studies how AI-related risks can be integrated into traditional financial model risk management processes.

The paper covers:

- Statistical tools for AI model risk measurement
- Sustainability, Accuracy, Fairness, and Explainability indicators
- Mapping SAFE indicators to financial risk categories
- Alignment with existing AI and financial risk management frameworks
- A nonlinear aggregate SAFE rating
- An illustrative credit scoring example

## Main Contributions

The main contribution of this paper is to connect AI model evaluation metrics with financial model risk management practices.

Specifically, the paper:

1. Explains how SAFE indicators can be measured using statistical tools.
2. Maps SAFE indicators to financial risk categories such as model risk, market risk, credit risk, regulatory risk, and governance risk.
3. Aligns the proposed framework with NIST AI RMF, ISO/IEC 23894:2023, the EU AI Act, Basel operational risk principles, and SR 11-7 model risk guidance.
4. Proposes a nonlinear aggregate SAFE rating using a weighted geometric mean.
5. Demonstrates the framework through an illustrative credit scoring model assessment.

## SAFE Dimensions

The paper focuses on four dimensions of AI risk:

| SAFE Dimension | Main Concern | Example Metrics / Tests |
|---|---|---|
| Sustainability | Model robustness and stability | Diebold-Mariano test, DeLong test |
| Accuracy | Predictive performance | RMSE, AUC, Diebold-Mariano test, DeLong test |
| Fairness | Bias across population groups | Gini coefficient, KS test, group-level AUC |
| Explainability | Transparency and interpretability | Shapley values, t-test |

## Statistical Tools Discussed

The paper introduces and applies several statistical tools, including:

- Diebold-Mariano test
- DeLong test
- Kolmogorov-Smirnov test
- t-test
- chi-squared test
- Gini coefficient
- Shapley values

These tools are used to compare forecasting errors, classification performance, distributions, feature importance, and explainability.

## Aggregate SAFE Rating

The paper proposes an aggregate SAFE rating using the weighted geometric mean:

```math
R_{\text{SAFE}} = S^{w_S} A^{w_A} F^{w_F} E^{w_E}
