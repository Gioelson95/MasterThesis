PMEmo Dataset - 2018/01



- The dataset consists of:
.
├── metadata.csv, song id, file name, song tile, artists
│ 
├── chorus.csv, song id, start time, end time
│ 
├── Annotations, the annotations for 794 songs in the dimension of valence and arousal
│   ├── Arousal
│   │   ├── 1-A.csv
│   │   ├── ...
│   │   └── 1000-A.csv
│   └── Valence
│       ├── 1-V.csv
│       ├── ...
│       └── 1000-V.csv
│ 
├── Chorus, 794 music clips (.MP3, chorus part)
│   ├── 1.mp3
│   ├── ...
│   └── 13.mp3
│ 
├── EDA, the electrodermal activity data of each subject for 794 songs
│   ├── Arousal
│   │   ├── 1_100177_A.csv
│   │   ├── ...
│   │   └── 1000_200378_A.csv
│   └── Valence
│       ├── 1_100177_V.csv
│       ├── ...
│       └── 1000_200378_V.csv
│ 
├── A_dynamic_mean.csv, the mean of dynamic labels in arousal
│ 
├── A_dynamic_std.csv, the standard deviation of dynamic labels in arousal
│ 
├── A_static.csv, the mean and the standard deviation of static labels in arousal
│ 
├── V_dynamic_mean.csv, the mean of dynamic labels in valence
│ 
├── V_dynamic_std.csv, the standard deviation of dynamic labels in valence
│ 
├── V_static.csv, the mean and the standard deviation of static labels in valence
│ 
├── dynamic_features.csv, 260 acoustic low-level descriptors of each 0.5 second for each song
│ 
└── static_features.csv, 6373 overall acoustic features of each song