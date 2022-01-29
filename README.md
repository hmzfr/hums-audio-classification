# Hums and Whistles Audio Classification

The data used in this project consists of participants humming and whistling to the
famous movie soundtracks (links to the soundtracks):

 - [**Hedwig's Theme (Harry Potter)**](https://www.youtube.com/watch?v=wtHra9tFISY)
 - [**The Imperial March (Star Wars)**](https://www.youtube.com/watch?v=B_iFRoJJLzc)
 - [**The Pink Panther Theme**](https://www.youtube.com/watch?v=VyZiIuMufTA)
 - [**Singin' in the Rain**](https://www.youtube.com/watch?v=StB2WR4Hwdo)
 - [**Hakuna Matata (The Lion King)**](https://www.youtube.com/watch?v=MBIWFTXQbi4)
 - [**Mamma Mia**](https://www.youtube.com/watch?v=unfzfe8f9NI)
 - [**This Is Me (The Greatest Showman)**](https://www.youtube.com/watch?v=CjxugyZCfuw)
 - [**Let It Go (Frozen)**](https://www.youtube.com/watch?v=L0MK7qz13bU)

As a result, there are 8 classes for the audio files.

The goals of this project are:
- Predict whether a sample belongs to the "Hedwig's Theme" or "The Imperial March" class (Binary classification).
- Predict the participant ID based on characteristics in their audio files (Multiclass classification).

## Motivation

Predicting a song label based on humming audio files of participants has many applications,
one of the most famous uses being the [**Shazam**](https://www.shazam.com/gb) app.
Predicting participant ID's is a very interesting concept, as if we are able to predict 
the identity of an individual based solely on their voice, this could have 
implications for personal privacy. It also may have uses in crime suspect investigation.
This project also identifies which models and features are the most important to
extract when working with audio files.

## Libraries

- [Librosa](https://librosa.org/doc/latest/index.html) (audio feature extraction)
- NumPy
- Pandas
- Matplotlib
- Sklearn


## Pipeline

Note: Nested K-Fold Cross-Validation was used to ensure reliable and accurate model
scores.

Algorithms used: SVM, KNeighbours, Logistic Regression, Extra Trees Classifier

![hw drawio](https://user-images.githubusercontent.com/50938851/151633170-05a22b7d-70dc-44e1-9907-7f5151f646ff.png)

## Results

A training accuracy of **0.93**, and test accuracy of **0.75** was obtained (when predicting
the identity of a participant). Therefore, some overfitting was observed (this is
explored in greater detail in the multiclass classification notebook).

