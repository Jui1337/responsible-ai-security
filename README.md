# Evaluating the Impact of Responsible AI as a Security Control in Machine Learning
This research explores whether applying **Microsoft's Responsible AI (RAI) principles** can improve the security of machine learning models. It compares a baseline model (built without RAI considerations) with a mitigated model (enhanced using RAI tools) to evaluate impact on security and robustness of machine learning model.

Adversarial testing is conducted using the **Adversarial Robustness Toolbox (ART)**, using two attacks customized for the tabular data.
- **Zeroth Order Optimization (ZOO) evasion attack**  
- **Label flip poisoning attack**

Dashboards are generated using **Microsoft's Responsible AI Toolbox** to visualize errors, fairness metrics, and interpretability.

The dataset used is the "Default of Credit Card Clients" from the **UCI Machine Learning Repository**.

## How to Use
Refer to the Jupyter notebooks for a complete flow from training to evaluation. To adapt this project to your own dataset or model:

- Replace the dataset loading section with your own dataset.
- If you're not using **XGBoost**, you can swap it with your preferred model (e.g., RandomForest, LightGBM, etc.).
- The dashboard integration using the Responsible AI Toolbox is already set up and can be reused with minimal modification.

This setup allows you to quickly plug in your own data and models while maintaining the same fairness, error, and explainability evaluation workflow.


