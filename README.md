# Parkinson-s-Disease-Detection

Parkinson's Disease (PD) is a chronic and progressive neurological disorder that primarily
affects movement. It occurs due to the degeneration of dopamine-producing neurons in a specific
area of the brain called the substantia nigra. The disease is characterized by symptoms such as
tremors, stiffness, bradykinesia (slowness of movement), and postural instability. Early
diagnosis of Parkinson's is crucial for managing symptoms and improving the quality of life of
patients. However, early detection is challenging due to the subtlety and overlap of early-stage
symptoms with other conditions.

Methodology:
1. Data Collection and Preprocessing:The dataset used for this project is the "Parkinson's Disease Classification" dataset,
which contains various acoustic features from individuals' speech samples. These
features include measures such as the average pitch, jitter, and shimmer of the voice,
which can serve as indicators of Parkinson's Disease.

2.Data Splitting:The dataset was split into training and testing sets using a 80-20 split. 80% of the data was
used for training the models, while the remaining 20% was reserved for testing and
evaluating model performance.

3. Handling Imbalanced Data:The dataset exhibited class imbalance, with more samples from individuals without
Parkinson's Disease than those with it. To handle this imbalance, the Synthetic Minority
Over-sampling Technique (SMOTE) was applied to generate synthetic samples for the
minority class, improving the models' ability to correctly predict the less-represented class.

4.Model Training:
 Five different machine learning models were trained on the data:
4.1 Support Vector Machine (SVM): A powerful classification technique that
finds the hyperplane that best separates the classes.
4.2 Decision Tree (DT): A non-linear model that splits the data into different
classes based on feature values.
4.3 Random Forest (RF): An ensemble method that builds multiple decision trees
and aggregates their predictions to improve accuracy and reduce overfitting.
4.4 AdaBoost: An ensemble method that combines multiple weak learners (like
decision trees) and adjusts the weights of incorrectly classified samples to improve
accuracу.
4.5 Artificial Neural Network (ANN): A deep learning model that simulates the
way the human brain processes information using layers of interconnected nodes.

5. Model Evaluation:Each model was evaluated using accuracy, loss, confusion matrices, and classification
reports. The performance of the models was visualized through accuracy and loss plots.
The confusion matrices were used to assess the number of true positives, true negatives,
false positives, and false negatives for each model, providing insights into how well the
model discriminates between classes.

6. Performance Comparison:The performance of the models was compared based on accuracy and loss values. The
models were also evaluated using confusion matrices, which allowed us to observe the
distribution of errors.
Visualizations like heatmaps were used to analyze the correlation between different features
and the target class (Parkinson's Disease or healthy), helping to identify important features
for classification.

7.Model Explanation:For each model, the feature importances were evaluated to provide insights into which
features most contributed to the prediction. For models like Random Forest and Decision
Trees, the importance of each feature in making predictions was plotted.
Model explanations, such as SHAP (Shapley Additive Explanations), could also be
considered for further interpretability.
