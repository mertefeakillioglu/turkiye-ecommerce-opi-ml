Perception-Based Online Purchase Behaviour Modelling in Turkish E-Commerce (ML & XAI)

This repository contains the complete reproducible codebase, dataset, modelling pipeline, and explainable AI analyses developed for the MSc dissertation:

“Factors Influencing Consumer Purchase Decisions in the Turkish E-Commerce Market: A Machine Learning-Based Feature Importance Analysis.”

The study models online purchase intention (OPI) as a behaviour-proximate probability using item-level perception data and analyses it through ensemble machine learning and Explainable Artificial Intelligence (XAI) techniques.

This repository is designed not as a simple code archive, but as a fully executable research environment.

🎯 Purpose of This Repository

This repository allows full reproduction of:

Data preparation steps

Model training and evaluation

SHAP global and class-level explainability

LIME local explanation analysis


The dataset used throughout this study is provided in the data/ directory as:

Survey on Consumer Decision Mechanisms in Online Shopping.xlsx

This file contains the original anonymised survey responses and serves as the starting point for all preprocessing and modelling steps described in Section 3.8 – Data Preparation.

📝 Survey Instrument

The original questionnaire structure, item wording, and measurement design are included in this repository to ensure transparency of how perception variables were operationalised before modelling.

▶️ Running the Analysis via Google Colab

All notebooks can be executed directly in the browser using Google Colab:

Colab Link:
https://colab.research.google.com/drive/1SR3z7UoRTolM38dWTtuOauttCQj7Ief2?usp=sharing

⬆️ Uploading the Survey Dataset in Colab

When the notebooks start in Colab, users are prompted to upload the survey dataset manually.

Simply upload:

Survey on Consumer Decision Mechanisms in Online Shopping.xlsx

from the data/ folder when prompted. The notebook then automatically proceeds with cleaning, encoding, modelling, and explainability steps.

This design ensures the analysis runs without any environment setup or file mounting.

🏆 Best Performing Configurations and Results

During experimentation, many model configurations and hyperparameter settings were tested.

For interpretability and behavioural clarity, the dissertation reports models that provided the most meaningful explanations rather than the absolute highest numerical scores.

The best-performing experimental results are included in this repository to ensure full transparency of the experimentation process and to demonstrate the trade-off between performance and interpretability.

🧪 Additional Analytical Outputs Beyond Thesis Figures

Not all generated SHAP, LIME, and evaluation visuals were included as figures in the dissertation.

They are provided here to document:

Robustness checks

Alternative class structure experiments

Additional explainability scenarios evaluated during model selection

This repository therefore documents the entire analytical exploration process, not only the final reported figures.

🔍 LIME Analysis Files — outputs/lime/

Local explanations showing how the model predicts for individual respondents.
| File                            | Explanation                         |
| ------------------------------- | ----------------------------------- |
| lime_high_binary.png            | High intention explanation (binary) |
| lime_low_binary.png             | Low intention explanation (binary)  |
| lime_misclassified_binary.png   | Misclassification analysis          |
| lime_all_classes_3class.png     | Overview (3-class)                  |
| lime_class_0_3class.png         | Low intention (3-class)             |
| lime_class_1_3class.png         | Mid intention (3-class)             |
| lime_class_2_3class.png         | High intention (3-class)            |
| lime_all_classes_multiclass.png | Overview (4-class)                  |
| lime_class_0_multiclass.png     | Very Low intention                  |
| lime_class_1_multiclass.png     | Low intention                       |
| lime_class_2_multiclass.png     | Medium intention                    |
| lime_class_3_multiclass.png     | High intention                      |

🌐 SHAP Analysis Files — outputs/shap/

Global and class-level explainability visuals.

| File                           | Explanation                    |
| ------------------------------ | ------------------------------ |
| shap_importance_binary.png     | Global importance (binary)     |
| shap_importance_multiclass.png | Global importance (4-class)    |
| shap_importance_3class.png     | Global importance (3-class)    |
| shap_summary_binary.png        | Summary plot (binary)          |
| shap_summary_multiclass.png    | Summary plot (4-class)         |
| shap_summary_3class.png        | Summary plot (3-class)         |
| shap_dependence_binary.png     | Dependence plot (binary)       |
| shap_dependence_multiclass.png | Dependence plot (4-class)      |
| shap_dependence_3class.png     | Dependence plot (3-class)      |
| shap_per_class_multiclass.png  | Per-class importance           |
| shap_per_class_3class.png      | Per-class importance (3-class) |
| shap_waterfall_binary.png      | Individual case (binary)       |
| shap_waterfall_multiclass.png  | Individual case (4-class)      |
| shap_waterfall_3class.png      | Individual case (3-class)      |

📈 Model Performance — outputs/results/

| File                          | Explanation           |
| ----------------------------- | --------------------- |
| binary_results.csv            | Binary model metrics  |
| multiclass_results.csv        | 4-class model metrics |
| multiclass_3class_results.csv | 3-class model metrics |
| confusion_matrices_3class.png | Confusion matrix      |

🔁 Reproducibility

By running the notebooks in order and using the provided dataset, all modelling steps, figures, and results from the dissertation can be reproduced.

👤 Author

Mert Efe Akillioglu
MSc Data Analytics
