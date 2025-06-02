# Audio_classifier_cnn

This personal project of mine is to practice classifying human non-speech audio using a 1D CNN. The model processes MFCC features extracted from each audio file and classifies them into categories like breath, cough, laugh, and more. 


Model performance so far:


Validation set accuracy: 79.57%


Test set accuracy: 64.55%


I plan to further improve it with data augmentation and advanced techniques.

## Dataset
I got the dataset from: [Nonspeech7k dataset](https://zenodo.org/records/6967442) (Rashid et al., 2023), containing 7,014 strongly labeled 32 kHz mono .wav files across 7 classes, which is used for this project.
