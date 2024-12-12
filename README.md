# Twitter Sentiment Analysis with PySpark

This project demonstrates a real-time Twitter sentiment analysis system using PySpark, Natural Language Processing (NLP), and Machine Learning (ML). It utilizes a Logistic Regression model to classify tweets as either positive or negative.

## Project Structure

- **`SENTIMENT.CSV`:** Dataset containing historical tweets and their sentiment labels (positive, negative). Replace with your own dataset or download a suitable one.
- **`code.py`:** (or your notebook file name) Main Python script containing the code for batch processing, model training, and real-time streaming.


## Getting Started

1. **Prerequisites:**
   - Python 3.6 or later
   - Java 8 or later
   - Spark 3.0 or later (pre-built for Hadoop 2.7 or later)
   - TextBlob
   - NLTK
2. **Install Dependencies:**
3. **Download NLTK Resources:**
4. **Run the Script:**

   ## Functionality

The project is divided into two parts:

**1. Batch Processing:**

- Reads tweet data from `SENTIMENT.CSV`.
- Preprocesses the tweets (tokenization, stop words removal, count vectorization, TF-IDF, label indexing).
- Trains a Logistic Regression model using PySpark's MLlib.
- Evaluates the model on a test set and prints the accuracy.

**2. Real-time Streaming:**

- Simulates a tweet stream using a socket server.
- Creates a Spark Streaming context to receive and process tweets.
- Applies the trained model to predict the sentiment of each incoming tweet.
- Prints the tweet text and predicted sentiment to the console.

## Notes

- The socket server is a basic simulation for demonstration purposes. In a real-world scenario, you would integrate with a real-time Twitter data source.
- The accuracy of the model depends heavily on the quality and size of the training dataset.
- Further improvements can be achieved by exploring more advanced ML models, incorporating sentiment lexicons, and handling sarcasm and irony.

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests.


## Acknowledgements

This project was inspired by various online resources and tutorials on Twitter sentiment analysis using PySpark.
