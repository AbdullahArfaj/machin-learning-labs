Project Summary: Iris Species Classification
This project uses a Support Vector Machine (SVM) to identify three types of iris flowers based on their measurements.

The Goal
Predict if a flower is a Setosa, Versicolor, or Virginica using four features:

Sepal length & width

Petal length & width

Step-by-Step Process
1. Data Visualization (EDA)
We look at the data first to find patterns.

Pairplots show that Setosa flowers are very different from the others and easy to identify.

KDE plots show where the measurements for specific flowers are most "crowded" or dense.

2. Preparation
We split the 150 samples into two groups:

Training Set (70%): Used to teach the model.

Test Set (30%): Used to "quiz" the model on data it hasn't seen yet.

3. Training the SVM
We use the SVC (Support Vector Classifier). It draws boundaries between the groups of flowers to separate them as clearly as possible.

4. Evaluation
We check the results using:

Confusion Matrix: A table showing which flowers the model got right and which ones it mixed up.

Accuracy Score: The percentage of correct guesses.

5. Tuning (GridSearchCV)
We fine-tuned the model by testing different settings for C (which handles errors) and Gamma (which handles how far the model looks for patterns).

Key Findings
The model reached 98% accuracy. Because the Iris dataset is very "clean," the model worked perfectly even with standard settings. However, the tuning process we used is a vital skill for harder, "messier" projects.
