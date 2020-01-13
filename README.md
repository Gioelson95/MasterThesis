# Master Thesis readme

The main idea is to take data from the PMEmo dataset for Music Emotion Computing and find better results in field of Music Emotion Recognition (MER).

PMEmo is a popular music dataset with emotional annotations: 

> It contain emotion annotations of 794 songs as well as the simultaneous electrodermal activity (EDA) signals. A Music Emotion Experiment was well-designed for collecting the affective-annotated music corpus of high quality, which recruited 457 subjects.  

Article: [The PMEmo Dataset for Music Emotion Recognition] (https://dl.acm.org/citation.cfm?id=3206037)

To briefly summarize, the PMEmo dataset provides:

* song metadata (song title, artists, beginning and ending timestamps of chorus section);
* manually selected music chorus clips (.mp3);
* pre-computed audio features for use in MER tasks;
* manually annotated emotion labels: static labels for the whole clips (i.e., overall labels), and dynamic labels for each 0.5-second segment (i.e., continuous labels over time);
* Corresponding EDA physiological signals;
* song lyrics (.lrc);
* song comments from online music websites (Chinese and English texts).

Whole dataset available at [here] (https://drive.google.com/drive/folders/1qDk6hZDGVlVXgckjLq9LvXLZ9EgK9gw0?usp=sharing)
the acoustic features and the annotations are all stored in CSV files
(delimited by comma).

The data about the features extraction etc. can be downloaded [here] (https://mega.nz/#F!b4MAzIBI!X9lQqEUzETixcimU0d6RCw)

In the `code` folder there are all the jupyter notebooks:
* `PMEmo_implementation`: code to get the same results of the PMEmo article
* `feature_extraction`: generation of .csv file with all songs features and EDA files.
  * `audio`:
    * `features`: explanation and visualization of all the audio features extracted
    * `features_extractor`: funcion that takes audio folder and return the .csv file with audio features
  * `eda`:
    * `eda_features`: explanation and visualization of all the eda features extracted
    * `eda_features_extractor`: funcion that takes eda folder and return the .csv file with eda features
* `feature_selection`: implementation of different algorithms of features selection based on the state of the art:
  1. Pearson correlation
  2. Backward elimination
  3. RFE (Recursive Feature Elimination)
  4. embedded method
  5. RreliefF algorithm
* `MER`: Music Emotion Recognition, where is evaluated performances in RMSE sense of various regressors based on audio, eda, combination of audio and eda and with no feature selection or different set of selected features.

---

Trying to reproduce article of [EDAGram] (https://ieeexplore.ieee.org/document/7590725), that implement a spectrogram for electrodermal activities, in `eda_gram folder`. This combinated with `spectrogram` folder will allow to use CNN neural networks based on EDA-Gram and spectrogram.


