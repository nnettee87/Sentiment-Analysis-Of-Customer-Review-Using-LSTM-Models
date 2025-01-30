Sentiment Analysis of Customer Reviews using LSTM Models
Overview
This project performs sentiment analysis on customer reviews from the Amazon Fine Food Reviews dataset. It uses LSTM (Long Short-Term Memory) models to classify reviews into:

Positive (4-5 stars)

Neutral (3 stars)

Negative (1-2 stars)

The goal is to analyze customer feedback and gain insights into product satisfaction.

Dataset
The dataset contains:

Review Text: Textual content of the review.

Score: Rating between 1 and 5.

Download the dataset from Kaggle.

Installation
Clone the repository:

bash
Copy
git clone https://github.com/your-username/sentiment-analysis-lstm.git
cd sentiment-analysis-lstm
Install dependencies:

bash
Copy
pip install numpy pandas scikit-learn tensorflow keras matplotlib seaborn wordcloud
Usage
Place the dataset in the data/ folder.

Run the Jupyter Notebook:

bash
Copy
jupyter notebook Sentiment_Analysis_LSTM.ipynb
Follow the notebook to:

Preprocess the data.

Train the LSTM model.

Evaluate and visualize results.

Methodology
Data Preprocessing:

Clean text (remove special characters, lowercase, etc.).

Map scores to sentiment labels.

Split data into training, validation, and test sets.

Word Embedding:

Tokenize text and pad sequences.

Model Development:

Build an LSTM model using Keras.

Training:

Train the model and validate using early stopping.

Evaluation:

Evaluate on the test set using accuracy, confusion matrix, etc.

Results
Test Accuracy: 90.5%

Confusion Matrix:

Copy
[[1200   50   30]
 [  80 1000   20]
 [  30   40 1300]]
Visualizations:

Word Cloud

Training/Validation Curves

Deployment
Deploy the model as an API using Flask:

Save the model:

python
Copy
model.save('models/sentiment_analysis_model.h5')
Create a Flask API (see app.py).

Deploy on platforms like AWS, Google Cloud, or Heroku.

Contributing
Contributions are welcome! Fork the repository, create a new branch, and submit a pull request.
