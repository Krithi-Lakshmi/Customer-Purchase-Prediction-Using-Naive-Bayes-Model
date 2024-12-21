# Customer-Purchase-Prediction-Using-Naive-Bayes-Model
Customer Purchase Prediction Using Naive Bayes Model

**Definition:**
The Naive Bayes model is a simple and effective machine learning algorithm based on Bayes' Theorem. 
It's called "naive" because it assumes that all features in the dataset are independent of each other 
(which might not always be true, but the model still performs well in many cases). It’s often used for classification tasks.

**How It Works:
Bayes' Theorem:**

It calculates the probability of something happening based on prior knowledge.
Formula:
𝑃(𝐴∣𝐵)=𝑃(𝐵∣𝐴)⋅𝑃(𝐴)/𝑃(𝐵)
 
𝑃(𝐴∣𝐵)
P(A∣B): Probability of A happening given B.

𝑃(𝐵∣𝐴)
P(B∣A): Probability of B happening given 𝐴.

𝑃(𝐴)
P(A): Probability of A.

𝑃(𝐵)
P(B): Probability of B.

**Naive Assumption:**

It assumes that each feature contributes independently to the probability of the outcome.

Use Case: Imagine you're classifying emails as "spam" or "not spam":

Features: Words like "free," "discount," "offer."

Target: Whether the email is spam or not.

**Explanation of Each Step**
**Importing Libraries:**

pandas: To create and manage the dataset.
sklearn: Provides tools for splitting data, encoding labels, and training the Naive Bayes model.

**Dataset Creation:**

The dataset includes age group, income level, and whether the product was purchased (target variable).

**Label Encoding:**

Since the Naive Bayes model cannot process strings, we convert categorical values (like "Young" and "Low") into numeric values using LabelEncoder.

**Splitting Data:**

The data is split into training (70%) and testing (30%) sets to evaluate the model.

**Training the Model:**

The GaussianNB class in scikit-learn is used to train the Naive Bayes model on the training data.

**Making Predictions:**

The trained model predicts whether customers in the test set purchased the product.

**Evaluating the Model:**

Accuracy: Percentage of correct predictions.
Classification Report: Detailed performance metrics like precision, recall, and F1-score.

**Similar Real-time Use Case :**

Customer Purchase Prediction:

Used to classify whether a customer will buy a product based on demographics and preferences.

Spam Detection:

Classify emails as spam or not spam based on word frequency.

Medical Diagnosis:

Predict diseases based on symptoms.

Sentiment Analysis:

Determine if a movie review is positive or negative.

