**Spam Detection using Logistic Regression**

This project aims to detect spam emails using a machine learning approach. We employ logistic regression on a dataset containing labeled email messages to classify them as either spam or ham (non-spam).

Dataset
The dataset used in this project is named "spam.csv". It consists of two columns: "class" and "message". The "class" column denotes whether the message is spam or ham, while the "message" column contains the text of the email.

**Preprocessing**

**Loading the Data:** The dataset is loaded into a Pandas DataFrame.

**Data Cleaning:** Any NaN values in the dataset are replaced with empty strings.

**Encoding Labels:** The labels in the "class" column are encoded to 0 for spam and 1 for ham.

**Train-Test Split:** The dataset is split into training and testing sets for model evaluation.

**Feature Extraction**

Text data is converted into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. This process converts the raw text into a matrix of TF-IDF features, which represents the importance of each word in the corpus.

**Model Training**

Logistic Regression, a popular classification algorithm, is trained on the TF-IDF features extracted from the training data.

**Model Evaluation**

The trained model is evaluated on both the training and testing datasets using accuracy score.

**Accuracy on Training Data**: 96.61%
**Accuracy on Test Data**: 96.23%

**Prediction**

Users can input their email message, and the trained model will predict whether it's spam or ham.

**Usage**

**Clone the Repository:** Clone this repository to your local machine.

**Install Dependencies:** Make sure you have all the required dependencies installed. You can install them using pip:

**pip install numpy pandas scikit-learn**

**Run the Script:** Run the provided Python script. It will load the trained model and prompt you to input your email message.

**Get Prediction:** After providing the input email message, the script will output whether it's classified as spam or ham.

**File Structure**

**spam.csv**: Dataset containing email messages and their labels.

**spam_detection.py**: Python script implementing the spam detection model and prediction functionality.

**README.md**: Documentation providing an overview of the project and usage instructions.

**Requirements**

Python 3.x
NumPy
pandas
scikit-learn

**Conclusion**

This project demonstrates the application of machine learning techniques for spam email detection. By training a logistic regression model on a labeled dataset, we can effectively classify email messages as spam or ham. This can be further extended and integrated into email services for real-time spam filtering.
