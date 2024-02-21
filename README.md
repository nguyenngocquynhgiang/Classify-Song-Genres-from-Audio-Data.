1. Overview

This project aims to classify music tracks into two genres, namely 'Hip-Hop' and 'Rock', using machine learning techniques. The classification is based on features extracted from the audio data of each track. The dataset used for this project is compiled by The Echo Nest, containing both metadata about the tracks and musical features such as danceability and acousticness.

2. Dataset Preparation

The dataset consists of two files in different formats: a CSV file containing track metadata and a JSON file with track acoustic metrics. To prepare the dataset, we merge these files into a single pandas DataFrame, retaining only relevant columns for further analysis.

3. Pairwise Relationships between Continuous Variables

We explore the relationships between different musical features using a correlation matrix and visualize it using a gradient background. This helps us identify any strong correlations between features which may affect our classification models.

4. Data Splitting

The data is split into training and testing sets, with features and labels separated accordingly. This ensures that our models are trained on one set of data and evaluated on another to assess their performance.

5. Normalizing the Feature Data

To avoid bias towards features with larger ranges of values, we normalize the feature data using standardization, ensuring that all features have a mean of 0 and a standard deviation of 1.

6. Principal Component Analysis (PCA) on Scaled Data

PCA is applied to reduce the dimensionality of the feature space while preserving most of the variance in the data. We visualize the explained variance by principal components to determine the optimal number of components to retain.

7. Training Classification Models

Two classification models, Decision Tree and Logistic Regression, are trained on the reduced-dimensional feature data. These models are then evaluated using performance metrics such as precision, recall, and F1-score.

8. Balancing the Data

Since the dataset is imbalanced with more 'Rock' tracks than 'Hip-Hop', we balance the data by subsetting an equal number of tracks from each genre. This ensures that the models are not biased towards the majority class.

9. Model Evaluation with Balanced Data
   
The decision tree and logistic regression models are retrained on the balanced dataset and evaluated to compare their performance. Cross-validation is applied to ensure robust evaluation of the models.

10. Conclusion

Based on the evaluation results, the logistic regression model appears to outperform the decision tree model in terms of accuracy on the balanced dataset. Further optimizations and model tuning can be explored to improve classification performance.
