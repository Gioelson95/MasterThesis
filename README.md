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

Whole dataset available at https://drive.google.com/drive/folders/1qDk6hZDGVlVXgckjLq9LvXLZ9EgK9gw0?usp=sharing
the acoustic features and the annotations are all stored in CSV files
(delimited by comma).

