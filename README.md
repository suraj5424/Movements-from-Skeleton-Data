### Task: Predicting Future Movements from Skeleton Data

#### Description:
Skeleton data analysis offers valuable insights into human movements and actions, facilitating applications such as fall detection and gesture recognition. This notebook tackles the challenge of predicting future movements based on past skeleton data, leveraging machine learning techniques. The dataset consists of time series of 3D skeleton data collected from individuals performing various activities.

### Data Information:
- The dataset comprises time series of 3D skeleton data collected from multiple subjects engaged in various activities.
- Each signal in the dataset is uniquely identified and consists of multiple lines of data, reflecting the temporal evolution of skeleton joint positions.
- The dataset is split into training and testing sets, with the training set containing labeled data for model training and the testing set requiring predictions to be submitted for evaluation.

### Solution Overview:
1. **Loading Data:** The data is downloaded from Kaggle and extracted. Necessary libraries are imported for data manipulation and modeling.
2. **Data Preprocessing:** Missing values are handled by filling them with the mean. The data is reshaped and prepared for training and testing.
3. **Model Training:** An XGBoost classifier is trained on the training set to predict future movements based on past skeleton data.
4. **Model Evaluation:** The trained model is evaluated on the test set to assess its accuracy.
5. **Making Predictions:** Predictions are made on the test data using the trained model.
6. **Submission File Creation:** Predicted classes are mapped to their corresponding labels and saved in a submission file for evaluation.

### Conclusion:
This script provides a solution to predicting future movements from skeleton data using an XGBoost classifier. By leveraging machine learning techniques, it addresses the challenge of understanding human movements and actions from time series of skeleton data. The predicted classes are formatted into a submission file for evaluation in the competition.
