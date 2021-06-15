# Sound-Track-Emotion-Recognition-Project---Classification

Description

The database contains 24 professional actors (12 female, 12 male), vocalizing two statements in a neutral North American accent. 
Speech includes calm, happy, sad, angry, fearful, surprise, and disgust expressions. 

Each expression is produced at two levels of emotional intensity (normal, strong), with an additional neutral expression. 

# No. of files

Data contains 1440 files or records: 60 trials per actor x 24 actors = 1440.

# Data Transformation and EDA
Sound features like the mfcc, chroma, and mel features that distinguish different sound characteristics like pitch(high or low), timbre (uniqueness of individual's voice) and power in voice were extracted to form dataset.

Different emotion samples were visualised, as well as the melspectogram sound feature - which is approximately a visualisation of sound by frequency.
Read more here --> https://en.wikipedia.org/wiki/Mel-frequency_cepstrum

# Modelling
After extracting several sound features, with the emotion of the file as the target variable, several classification models were tried:

1. LogisticRegression
2. LogisticRegression with Ridge Penalty (l2)
3. LogisticRegression with Lasso Penalty (l1)
4. Support Vector Machine
5. Random Forest

# Model Metrics - accuracy.
The best model at predicting emotion was the Support Vector Machine (hyper parameters: "rbf" kernel, c=10),  at overall accuracy of 82%.


