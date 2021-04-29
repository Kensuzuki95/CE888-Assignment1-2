# CE888 Project 2: TweetEval tweet classification tasks

This Github Repository contains original codes and preprocessed datasets used in the CE888 Assignement 2 Paper[Title: Performance Evaluation of A Lite BERT (ALBERT)
and LSTM on Multi-Class Tweet Classification Task under Lower Computational Environment](https://drive.google.com/file/d/1zRfJUGnegm-Ilbybi9d7UPwIQKA1qRNr/view?usp=sharing). 

## The Description of Jupyter Notebooks

This GitHub Repository contains 4 Jupyter Notebooks and details are shown below:

A. [`TweetEval_Datasets_Emoji,_Emotion,_Sentiment.ipynb`](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Datasets_Emoji%2C_Emotion%2C_Sentiment.ipynb)
 - This jupyter notebook shows the preprocessing process. The Datasets shared in this GitHub Repositary are the preprocessed datasets produced in this Jupyter Notbook.

B. [`TweetEval_Emoji_LSTM_or_ALBERT.ipynb`](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Emoji_LSTM_or_ALBERT.ipynb)
 - Contains codes to conduct `Emoji Prediction` tasks from TWEETEVAL

C. [`TweetEval_Emotion_LSTM_or_ALBERT.ipynb`](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Emotion_LSTM_or_ALBERT.ipynb)
 - Contains codes to conduct `Emoji Prediction` tasks from TWEETEVAL

D. [`TweetEval_Sentiment_LSTM_or_ALBERT.ipynb`](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Sentiment_LSTM_or_ALBERT.ipynb)
 - Contains codes to conduct `Sentiment Analysis` tasks from TWEETEVAL

*The original source of the tweet text data are used in the TWEETEVAL paper by [Barbieri et al. (2020)](https://www.aclweb.org/anthology/2020.findings-emnlp.148.pdf), and for further detailed information of the three TWEETEVAL-based tasks is available in the paper. 

## The Description of the Preprocessed Datasets (Listes as CSV files)

- **Emoji Datasets**: Used for Emoji Prediction task and each tweet text is labled into either of the 20 labels: :heart:, :heart_eyes:, :joy:  `...` :evergreen_tree:, :camera:, :stuck_out_tongue_winking_eye:
  - [Train Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/df_emoji_train.csv): 42,631 Tweets
  - [Validation Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/commit/78cc9a0ad9a27913b48f8c83e9f18394578e504c): 4,471 Tweets
  - [Test Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/commit/78cc9a0ad9a27913b48f8c83e9f18394578e504c): 48,764 Tweets
- **Emotion Datasets**: Used for Emotion Recognition task and each tweet text is labled into either of the 4 labels `anger`, `joy`,`sadness`, `optimism`
  - [Train Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/commit/607eee3598788f428908d8998f3d647614e0c55b): 3,257 Tweets
  - [Validation Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/commit/607eee3598788f428908d8998f3d647614e0c55b): 372 Tweets
  - [Test Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/commit/607eee3598788f428908d8998f3d647614e0c55b): 1,421 Tweets
- **Sentiment Datasets**: Used for Sentiment Analysis task and each tweet text is labled into either of the 3 labels: `positive`, `neutral`, `negative`
  - [Train Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/df_sentiment_train.csv): 36,373 Tweets 
  - [Validation Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/df_sentiment_val.csv): 1,623 Tweets
  - [Test Dataset](https://github.com/Kensuzuki95/CE888-Assignment1-2/commit/607eee3598788f428908d8998f3d647614e0c55b): 12,032 Tweets

*If you want to check the original source of each datasets, please visit the [TWEETEVAL GutHub Repository](https://github.com/cardiffnlp/tweeteval) 

## Instruction for Executing TWEETEVAL Tasks: Emoji Prediction, Emotion Recognition, and Sentiment Analysis

1. Open the jupyter notebook according to the task that you want execute. ([Emoji Prediction](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Emoji_LSTM_or_ALBERT.ipynb), [Emotion Recognition](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Emotion_LSTM_or_ALBERT.ipynb), [Sentiment Analysis](https://github.com/Kensuzuki95/CE888-Assignment1-2/blob/main/TweetEval_Sentiment_LSTM_or_ALBERT.ipynb))
2. Modify the codes based on your preference to load the required train / validation / test datasets
  - The original codes exracts the data from a personal GoogleDrive
  - Please either downloand the dataset from this GitHub Repository or use the link to directly import the data
3. Run the codes accordingly
  - Use of GPU Runtime on GoogleColab is highly recommended when running the codes 
  - Processing the training datasets may take several hours (for Emoji Prediction and Sentiment Analysis) due to large size of corpus
  - Feel free to test your model on new texts by modifying the `Testing the Model` section after training and testing the created models
