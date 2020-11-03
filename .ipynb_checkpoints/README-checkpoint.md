# Musical Genre Classifier
Three Musical genre classifiers were implemented.
* A CNN with [MFCCs](https://en.wikipedia.org/wiki/Mel-frequency_cepstrum) as the input (worst performance)
* A CNN with a mel spectrogram as the input
* [GXBoost](https://xgboost.readthedocs.io/en/latest/) with nearly all features from [essentia](https://essentia.upf.edu/index.html) as the input (best performance)

# Dataset
The provided dataset consisted out of four genres with roughly 11 songs per genre. Part of the task was it to split the songs into 30 second clips with resulted in roughly 10 clips per song.

# Results
Due to the limited dataset provided the results may not be indicative of the perfermance on a larger / more diverse dataset. If not otherweise noted the data was randomly shuffled and split 75:25 between training and testing.

![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/CM_MFCC.JPG?raw=true)\
Above the confusion Matrix of the CNN on the MFCCs (Overall 63%). 
\
\
![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/CM_Mel.JPG?raw=true)\
Above the confusion Matrix of the CNN on the Mel spectrogram (Overall 85%). 
\
\
![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/CM_XGBoost.JPG?raw=true)\
Above the confusion Matrix of the XGBoost on the essentia features (Overall 93%). When picking two songs per genre for testing so that the classifier had not seen any clips of these songs before the overall accuracy droped to 90%.
\
\
![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/Features_XGBoost.JPG?raw=true)
Top ten features used by XGBoost for classification. It can be seen that the bpm histogram has by far the largest influence on the classification.