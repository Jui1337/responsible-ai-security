# Evaluating Microsoft Responsible AI as Defense Against Label Flip and ZOO Attacks
This project investigates whether applying **Microsoft's Responsible AI (RAI) principles** can improve the security and robustness of machine learning models on **tabular data**.

Comparison involves:
- A **baseline model** (trained without RAI considerations), and
- An **RAI-enhanced model** (developed using RAI practices like fairness assessment, error analysis, and transparency).

To evaluate robustness, **Adversarial Robustness Toolbox (ART)** is used with the two attacks customized for tabular data:
- **Zeroth Order Optimization (ZOO)** evasion attack  
- **Label flip poisoning** attack

For the baseline model, **post-attack defenses** are applied:
- **ZOO**: High-confidence prediction filtering  
- **Label flip**: Noisy label detection via **Cleanlab** and outlier filtering using **Isolation Forest**

The **RAI-enhanced model** does not use these reactive defenses but is designed using RAI principles from the start. This allows fair comparison of **RAI-driven robustness** with traditional defensive techniques in adversarial scenarios.

Dashboards are generated using **Microsoft's Responsible AI Toolbox** to visualize errors, fairness metrics, and interpretability.

The dataset used is the "Default of Credit Card Clients" from the **UCI Machine Learning Repository**.

## How to Use
Refer to the Jupyter notebooks for a complete flow from training to evaluation. To adapt this project to your own dataset or model:

- Replace the dataset loading section with your own dataset.
- If you're not using **XGBoost**, you can swap it with your preferred model (e.g., RandomForest, LightGBM, etc.).
- The dashboard integration using the Responsible AI Toolbox is already set up and can be reused with minimal modification.

This setup allows you to quickly plug in your own data and models while maintaining the same fairness, error, and explainability evaluation workflow.

## Installation

Before running the notebooks, install all required dependencies by running:

```bash
pip install -r requirements.txt

## Acknowledgment

This code was developed for the research project titled  
**"Evaluating Microsoft Responsible AI as Defense Against Label Flip and ZOO Attacks"**  
by **Jui Bangali**, under the guidance of **Professor Brent Lagesse**,  
as part of the Master's in Cybersecurity Engineering program at the **University of Washington, Bothell**.

