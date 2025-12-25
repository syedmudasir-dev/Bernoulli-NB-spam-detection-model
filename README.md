Restaurant Review Sentiment Analysis
This project demonstrates a complete machine learning workflow to classify restaurant reviews as positive or negative. It utilizes text preprocessing techniques and a Bernoulli Naive Bayes model to achieve sentiment classification.

📊 Dataset
The project uses the Restaurant Reviews dataset from Kaggle (rahulbanerj24/resturant-reviews).

Total Records: 1,000 reviews.

Columns:

Review: The text of the customer review.

Liked: A binary label where 1 indicates a positive review and 0 indicates a negative one.

🛠️ Requirements
The following Python libraries are required to run this notebook:

pandas

nltk

scikit-learn

kagglehub (for dataset downloading)

🚀 Project Workflow
1. Data Acquisition & Cleaning
Download: The dataset is fetched directly from Kaggle using the kagglehub library.

Preprocessing: A custom text cleaning function is implemented to:

Remove punctuation marks using the string library.

Remove common English stopwords using nltk.

2. Feature Extraction
Bag of Words (BoW): The notebook utilizes CountVectorizer from scikit-learn to convert cleaned text into a numerical format (sparse matrix).

Vocabulary: The resulting vocabulary consists of approximately 2,240 unique words.

3. Model Training & Evaluation
Model: A Bernoulli Naive Bayes classifier (BernoulliNB) is trained on the vectorized review data.

Performance: The model achieved an accuracy score of 72% on the test dataset.

4. Testing on Unseen Data
The notebook includes a section to test the model against new, manually entered reviews. For example, the review "Ample Portions and good prices" can be transformed and predicted by the model.
