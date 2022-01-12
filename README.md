# speech-recognition

In this project, I used the Common Voice dataset on English-speaking data. I downloaded the data from Kaggle (https://www.kaggle.com/mozillaorg/common-voice).

## Gender classification
The first task I carried out was to classify gender based on the voice of the speaker. For this, I used a single feature - the mean pitch level (as estimated by the Pyin algoriothm available in librosa) - and applied an optimization function to find the best threshold value for the feature.

Using 120 frames for the optimization procedure (i.e. training), and applying the resulting threshold on 80 testing frames, I obtain an accuracy of ~90/95%. 
