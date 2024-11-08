Student Purchase Prediction - Data Preprocessing and Machine Learning
Overview
This project aims to predict the likelihood of a student, registered for a free plan, purchasing a subscription on our platform. The decision is based on students' activities, such as viewing lectures and participating in exams. By predicting student purchases, the goal is to improve targeting strategies, particularly in cases like Black Friday campaigns, to retarget students with tailored ads on social media.

Business Case
The business case behind this project stems from the desire to improve business decision-making through machine learning. In 2022, 365 launched a predictive initiative aimed at forecasting student purchases prior to the Black Friday campaign. The challenge was to identify students likely to purchase a subscription and target them with special ads.

Problem
The main challenge in this case is the class imbalance in the data. The number of students who had never purchased a subscription significantly outnumbered those who had. This imbalance was primarily due to a free campaign conducted before Black Friday, where all 365 students were granted free access to the platform.

Implication
Predicting student purchases in such a scenario is a difficult task because of two main factors:

Class Imbalance: The vast majority of students did not make a purchase, which makes it harder for machine learning models to detect patterns in the minority class (students who did purchase).
Unpredictable Human Behavior: Student purchasing behavior can be influenced by a variety of factors, many of which are difficult to capture accurately with the available features, further complicating predictions.
Data Preprocessing
The project involved preprocessing the available data before training machine learning models. This step included:

Handling Missing Values: Missing data was cleaned and appropriately imputed.
Feature Engineering: Relevant features were created based on students’ activities on the platform, such as the number of lectures viewed, exams attempted, etc.
Balancing the Dataset: Techniques like oversampling, undersampling, or using algorithms that handle imbalanced classes were explored to address the imbalance in the data.
Scaling: Features were normalized or scaled to ensure consistency and avoid bias in models sensitive to feature scaling.
Machine Learning Models
Multiple machine learning models were tested to predict student purchase likelihood. These models were trained on a variety of features such as:

Lecture Views
Exams Participated
Platform Interaction (time spent, engagement)
The following models were considered:

Logistic Regression
Random Forest Classifier
Support Vector Classifier (SVC)
K-Nearest Neighbors (KNN)
Challenges Encountered
Imbalanced Dataset: As mentioned, class imbalance made it difficult for models to predict the minority class (students likely to purchase) effectively.
Feature Selection: Determining which features contributed the most to the prediction was another challenge, given the potential high correlation between features such as time spent on the platform and course activity.
Model Evaluation
Performance was evaluated using common metrics like accuracy, precision, recall, and F1-score, with a focus on the recall metric for the minority class (purchased subscriptions). Techniques like cross-validation and grid search were employed to fine-tune hyperparameters and ensure the models generalized well to unseen data.
