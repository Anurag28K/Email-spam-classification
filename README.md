📧 Spam Email Classification
The Spam Email Classification project aims to detect offensive and anti-social elements in emails, suspect them, and block them, thereby identifying suspicious users. Suspicious email detection involves identifying users by determining the keywords they use, such as "bomb" or "RDX", found in their emails. Blocked emails are then checked by the administrator to identify the users who sent such emails.

Overview
The provided code implements a spam email classifier using the Logistic Regression algorithm. It utilizes the "spam.csv" dataset, containing labeled messages as either "spam" or "ham" (not spam). The data is preprocessed to handle missing values and map labels to numerical values.

The text data is transformed into numerical features using TF-IDF Vectorization, converting each message into a vector of term frequency-inverse document frequency values. The dataset is then split into training and testing sets, with 80% for training and 20% for testing.

A Logistic Regression model is trained on the training data, achieving around 96.6% accuracy on the training data and 96.2% accuracy on the test data.
