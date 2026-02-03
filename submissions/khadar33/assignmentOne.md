Research Assignment: Introduction to Machine Learning
1. Definition of Machine Learning with a Real-Life Example
Machine Learning (ML) is a part of Artificial Intelligence (AI) that lets computers learn
from experience and get better at tasks over time, much like how people improve with
practice. Instead of being given exact instructions for every situation, computers use the
patterns they find in data to make predictions and decisions on their own.
Real-Life Example: Movie Recommendations (Netflix/YouTube)
Netflix and YouTube don’t follow fixed rules. Instead, they learn from what you watch,
like, or skip. The system gradually learns patterns in viewing behavior, such as favorite
genres, preferred actors, or typical viewing times, and uses this information to suggest
movies or videos a user is likely to enjoy.
2. Supervised vs. Unsupervised Learning
Supervised Learning:
 Works with data that already has answers or labels.
 The system learns by comparing its predictions with the correct results and
improving over time.
 Common tasks include predicting numbers (regression) or classifying items into
categories (classification).
 Example: Predicting house prices based on size, location, and number of rooms,
or detecting whether an email is spam or not.
Unsupervised Learning:
 Works with data that has no labels or answers.
 The system explores the data to find hidden patterns, relationships, or groups on
its own.
 Common tasks include clustering similar items, segmenting customers, or
simplifying complex datasets (dimensionality reduction).
 Example: Detecting unusual transactions in a bank to find potential fraud, or
grouping articles by topics in a news website.
Comparison TableAspect Supervised Learning Unsupervised Learning
Data Type Labeled (input + known
output) Unlabeled (input only)
Goal Predict outcomes Discover hidden patterns or
groups
How it
Learns
Compares predictions with
correct answers
Finds patterns or similarities
without answers
Common
Tasks Regression, Classification Clustering, Dimensionality
Reduction
Example Predicting house prices, Spam
detection
Detecting fraud, Grouping
articles by topic
3. Overfitting: Causes and Prevention
Overfitting happens when a model learns the training data too closely, including small
mistakes or random details, instead of learning the general pattern.
Causes: It usually happens when the model is too complicated, the training data is too
small, or the data has irrelevant or unusual details.
Prevention Strategies: To prevent overfitting, we can simplify the model, use more or
better-quality data, check the model on new data, and stop training before it starts
memorizing unimportant details.
4. Training Data vs Test Data Split
Training Data vs Test Data Split
Machine learning models need to be tested on data they haven’t seen before to check if
they can generalize. That’s why datasets are split into:
 Training data (70–80%): Used by the model to learn patterns from the data.
 Test data (20–30%): Used to evaluate how well the model performs on new,
unseen data.
This ensures the model isn’t judged only on the data it was trained on, which could give
misleading results.
Example: If we want to predict whether a customer will buy a product, we might use
800 past customer records for training and 200 new records for testing. If the modelperforms well on both, it is likely generalizing; if it only works on the training data, it is
overfitting.
5. Case Study: Machine Learning Case Studies in Transportation
Case Study Title: “Predicting Public Transport Ridership Loss Using Machine Learning”
(European Transport Research Review, 2025)
Summary:
Researchers used machine learning to predict how bus ridership in Stockholm changed
during crises like the COVID-19 pandemic. They wanted to estimate how many
passengers would stop using buses and the financial impact of these changes.
Algorithms tested: Decision Trees, Random Forests, Neural Networks, Support Vector
Regression, and k-Nearest Neighbors (kNN).
Best result: k-Nearest Neighbors (kNN) gave the most accurate predictions.
Findings: The study found that ridership dropped by 49% in 2020 and 82% in 2021.
The machine learning models could identify patterns in passenger behavior that
traditional methods often miss.
Impact:
This work shows how machine learning can help city planners and public transport
authorities make better decisions during crises, such as adjusting bus schedules,
managing resources, and planning budgets more effectively.
References
1. European Transport Research Review. (2025). Predicting public transport
ridership loss using machine learning. SpringerOpen.
https://etrr.springeropen.com/articles/10.1186/s12544-025-00722-z
2. Geron, A. (2019). Hands-On Machine Learning with Scikit-Learn, Keras, and
TensorFlow (2nd ed.). O’Reilly Media.
3. Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning. MIT Press.
4. Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical
Learning: Data Mining, Inference, and Prediction (2nd ed.). Springer.
5. Russell, S., & Norvig, P. (2020). Artificial Intelligence: A Modern Approach (4th
ed.). Pearson.6. Lifewire. (2023). What is supervised learning? Lifewire.
https://www.lifewire.com/what-is-supervised-learning-7508014
