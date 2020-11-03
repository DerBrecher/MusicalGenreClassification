# Musical Genre Classifier
Three Musical genre classifiers were implemented.
* A CNN with [MFCCs](https://en.wikipedia.org/wiki/Mel-frequency_cepstrum) as the input
* A CNN with a mel spectrogram as the input
* [GXBoost](https://xgboost.readthedocs.io/en/latest/) with nearly all features from [essentia](https://essentia.upf.edu/index.html) as the input

# Results

![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/CM_MFCC.JPG?raw=true)\
Confusion Matrix of the CNN on the MFCCs. 
\
\
![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/CM_Mel.JPG?raw=true)\
Confusion Matrix of the CNN on the Mel spectrogram. 
\
\
![alt text](https://github.com/DerBrecher/MusicalGenreClassification/blob/master/images/CM_XGBoost.JPG?raw=true)\
Confusion Matrix of the XGBoost on the essentia features.