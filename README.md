###  Music Genre Classification with Machine Learning


Music lovers often have vast collections with songs spanning various genres. Manually organizing these songs can be time-consuming. This project offers a solution by leveraging the power of machine learning to automate genre classification.

The project will explore a dataset containing song metadata (titles, artists, genres) and corresponding audio features (danceability, energy, etc.). By analyzing these features, the model will learn to identify patterns that distinguish between different genres.
![image](https://github.com/nguyenngocquynhgiang/Classify-Song-Genres-from-Audio-Data./assets/135851627/5597f86c-34a8-4a6c-ab7c-250bb6b0a42b)

1. **Load the data:** The data consists of two parts: track metadata (including titles, artists, and genre labels) and audio metrics (like danceability and energy) for each track. Pandas is used to load this data from CSV and JSON files and merge them into a single DataFrame.

2. **Explore the data:** This involves checking for missing values, data types, and getting an overall idea of the data's distribution.

![image](https://github.com/nguyenngocquynhgiang/Classify-Song-Genres-from-Audio-Data./assets/135851627/50e2a43c-88fe-477f-aa81-459d136c45eb)

3. **Identify relationships between features:** The report examines how different audio metrics correlate with each other. For example, high acousticness might indicate a slower tempo and lower energy.
![image](https://github.com/nguyenngocquynhgiang/Classify-Song-Genres-from-Audio-Data./assets/135851627/fe99ea2e-74a2-48dc-a9c7-3832b53dfef0)

4. **Split the data:** The data is split into two sets: training data for training the machine learning model and test data for evaluating the model's performance.
![image](https://github.com/nguyenngocquynhgiang/Classify-Song-Genres-from-Audio-Data./assets/135851627/bb665e20-4618-40a7-80ce-0c2515cf0ae8)

5. **Normalize the data:** This ensures all features have a similar range of values, which can improve the performance of some machine learning algorithms.
![image](https://github.com/nguyenngocquynhgiang/Classify-Song-Genres-from-Audio-Data./assets/135851627/00269b5b-6c15-4a64-8db4-2b6c394a307e)

6. **Apply dimensionality reduction (PCA):** Principal Component Analysis (PCA) is used to reduce the number of features while retaining most of the important information in the data. This can be helpful for improving model performance and reducing training time.

7. **Train machine learning models:** Here, the report uses two models: decision tree and logistic regression. Both models are trained on the preprocessed training data to learn how to classify songs based on their audio features.

8. **Evaluate model performance:** The models' performance is evaluated using classification reports, which provide metrics like precision, recall, and F1-score for each genre classification.

9. **Compare models:** The report compares the performance of the decision tree and logistic regression models and identifies which one performs better for this specific task.

10. **Balance the data:** The dataset might be imbalanced, with more data points for one genre (e.g., rock) than another (e.g., hip-hop). This can bias the model towards the majority class. The report addresses this by creating a balanced dataset with an equal number of data points for each genre.

11. **Evaluate impact of balancing:** The report trains the models again using the balanced dataset and compares the performance with the imbalanced dataset. This helps to assess whether balancing the data improves model bias and overall classification accuracy.

Overall, this report provides a step-by-step explanation of how to prepare and analyze data for music genre classification using machine learning techniques. It highlights the importance of data cleaning, exploration, dimensionality reduction, and model selection for achieving good classification performance.

The successful outcome of this project will be a machine learning model that can automatically classify songs into their respective genres based on their audio properties. This model has the potential to be integrated into music streaming platforms or personal music libraries to simplify music organization and enhance user experience. 
