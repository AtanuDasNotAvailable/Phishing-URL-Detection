<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Phishing URL Detection Project</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
            margin: 20px;
        }
        h1, h2 {
            text-align: left;
        }
        h1 {
            margin-bottom: 15px;
        }
        h2 {
            margin-top: 30px;
            margin-bottom: 15px;
        }
        ul {
            margin: 10px 0 20px 40px;
        }
        code {
            background-color: #eaeaea;
            padding: 2px 6px;
            border-radius: 4px;
        }
        .section {
            background-color: #fff;
            padding: 20px;
            margin-bottom: 25px;
            border-radius: 10px;
            box-shadow: 0 0 8px rgba(0,0,0,0.05);
        }
    </style>
</head>
<body>
    <h1>Phishing URL Detection Project</h1>
    <p class="section">
        This project presents a comprehensive machine learning pipeline to classify phishing URLs using multiple classifiers, data preprocessing techniques, and evaluation metrics.
    </p>

    <h2>📂 Project Overview</h2>
    <div class="section">
        <p>The pipeline involves:</p>
        <ul>
            <li>Fetching and preparing the dataset using the <code>ucimlrepo</code> package.</li>
            <li>Addressing class imbalance with techniques like <strong>SMOTE</strong>, <strong>ADASYN</strong>, and <strong>Borderline SMOTE</strong>.</li>
            <li>Feature selection using <code>SelectKBest</code> with ANOVA F-test.</li>
            <li>Model training with multiple classifiers:
                <ul>
                    <li><strong>Random Forest</strong></li>
                    <li><strong>SVM</strong></li>
                    <li><strong>Logistic Regression</strong></li>
                    <li><strong>Decision Trees</strong></li>
                    <li><strong>XGBoost</strong></li>
                    <li><strong>KNN</strong></li>
                    <li><strong>Gradient Boosting</strong></li>
                    <li><strong>StackingClassifier</strong> (ensemble of multiple base learners)</li>
                </ul>
            </li>
            <li>Evaluation using:
                <ul>
                    <li>Accuracy</li>
                    <li>ROC AUC</li>
                    <li>Confusion matrix</li>
                    <li>Classification report</li>
                </ul>
            </li>
            <li>Model interpretability with <strong>LIME</strong>.</li>
        </ul>
    </div>

    <h2>🧰 Tools & Libraries</h2>
    <div class="section">
        <ul>
            <li><strong>Python 3.x</strong></li>
            <li>pandas, numpy</li>
            <li>seaborn, matplotlib</li>
            <li>scikit-learn</li>
            <li>imbalanced-learn</li>
            <li>xgboost</li>
            <li>lime</li>
            <li>ucimlrepo</li>
        </ul>
    </div>

    <h2>📈 Model Pipeline</h2>
    <div class="section">
        <ol>
            <li><strong>Data Loading</strong> from UCI repository</li>
            <li><strong>Data Preprocessing</strong>:
                <ul>
                    <li>Label encoding</li>
                    <li>Scaling</li>
                </ul>
            </li>
            <li><strong>Class Balancing</strong>:
                <ul>
                    <li>SMOTE, ADASYN, BorderlineSMOTE</li>
                </ul>
            </li>
            <li><strong>Feature Selection</strong>:
                <ul>
                    <li><code>SelectKBest(f_classif)</code></li>
                </ul>
            </li>
            <li><strong>Model Training</strong>:
                <ul>
                    <li>RandomForest, SVM, LogisticRegression, etc.</li>
                </ul>
            </li>
            <li><strong>Evaluation</strong>:
                <ul>
                    <li>Metrics + LIME explanations</li>
                </ul>
            </li>
        </ol>
    </div>
   <h2> Feel free to explore the notebooks and results for a detailed breakdown of the process and performance.</h2>
</body>
</html>
