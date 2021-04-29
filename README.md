# CE888 Project 2: TweetEval tweet classification tasks

This Github Repository contains original codes and preprocessed datasets used in the CE888 Assignement 2 Paper[Title: Performance Evaluation of A Lite BERT (ALBERT)
and LSTM on Multi-Class Tweet Classification Task under Lower Computational Environment](https://drive.google.com/file/d/1zRfJUGnegm-Ilbybi9d7UPwIQKA1qRNr/view?usp=sharing). 

## The Description of Jupyter Notebooks

The `TweetEval_Datasets_Emoji,_Emotion,_Sentiment.ipynb` contains codes for assignemnt 1. There are mainly 3 contents in the jupyter notebook file:
1. Load the Datasets for `emoji`, `emotion`, and `sentiment` from Tweeteval dataset accessible from following githib page (URL: https://github.com/Kensuzuki95/tweeteval.git)
2. Check the content of 3 datasets in each test, train, validation data [size, label category, train-test-split ratio]
3. Conduct basic preprocessing on the datasets

All data are accessible from the Tweeteval github page, I have loaded my date via Google Drive by downloading the datasets from the github page and uploading to my personal drive.

## The Description of the Preprocessed Datasets (Listes as CSV files)

- **Emoji Datasets**: Used for Emotion Recognition task and each tweet text is labled into either of the 20 labels: :heart:, :heart_eyes:, :joy:  `...` :evergreen_tree:, :camera:, :stuck_out_tongue_winking_eye:
- **Emotion Datasets**: Used for Emotion Recognition task and each tweet text is labled into either of the 4 labels `anger`, `joy`,`sadness`, `optimism`
- 

