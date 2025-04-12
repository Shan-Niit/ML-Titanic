# ML-Titanic
Explored Titanic survival prediction with baseline, binned, and full feature sets. Applied PCA for dimensionality reduction. Best accuracy (0.8202) from GradientBoosting with all features. PCA helped MLP but lowered other models’ scores.


Titanic Classification – Feature Engineering, Model Selection & PCA
This project explores multiple machine learning strategies to solve the Titanic survival prediction challenge. It focuses on feature engineering, model evaluation, and dimensionality reduction using PCA — with the goal of maximizing accuracy and building a strong ML pipeline.

✅ Project Overview
The pipeline involves:

Custom feature creation

Baseline and advanced model comparison

Evaluation of different feature configurations

Dimensionality reduction via PCA

Final model selection for production

⚙️ Feature Set Testing
We evaluated three configurations of the dataset to understand how engineered features affect model performance:

Version	Description
Version 1 – Baseline	All features included except Fare, Age, FareBin, and AgeBin
Version 2 – Binned Only	Included only binned versions of Fare and Age (FareBin, AgeBin)
Version 3 – All Features	Full feature set including both original and binned versions of Fare and Age
📊 Accuracy Comparison (No PCA)
🔹 Version 1 – Baseline (No Fare / Age / Binned)
Model	Accuracy
SVC	0.7921
RandomForest	0.7978
XGBoost	0.7921
MLP	0.8034
KNN	0.7640
DecisionTree	0.7865
ExtraTrees	0.7978
GradientBoosting	0.7978
VotingClassifier	0.8202
🔹 Version 2 – Binned Only
✅ Best Accuracy: XGBoost – 0.7921

🔹 Version 3 – All Features
Model	Accuracy
SVC	0.7865
RandomForest	0.7697
XGBoost	0.8034
MLP	0.7753
KNN	0.7978
DecisionTree	0.8202
ExtraTrees	0.8034
GradientBoosting	0.8202
VotingClassifier	0.8146
🧠 Final Feature Strategy
Strategy	Best Model	Accuracy
Baseline	VotingClassifier	0.8202
Binned Only	XGBoost	0.7921
All Features	GradientBoosting / DecisionTree	0.8202
➡️ Conclusion: The best overall results came from using all features (original + binned), offering the most flexibility and top-tier accuracy.

🧪 PCA – Dimensionality Reduction Test
We applied PCA to reduce dimensionality and evaluated its impact on performance:

Model	Accuracy (PCA)
SVC	0.7921
RandomForest	0.7697
XGBoost	0.7753
MLP	0.8146
KNN	0.7921
DecisionTree	0.7978
ExtraTrees	0.7697
GradientBoosting	0.7640
VotingClassifier	0.7978
➡️ PCA generally led to a slight drop in accuracy, except for MLP, which benefited from dimensionality reduction.

🔍 Visualize feature importance from top models

🌀 Plot 2D PCA components to explore separation

📈 Create visual comparisons of model performances

