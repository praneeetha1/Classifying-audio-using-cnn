# Audio_classifier_cnn

This personal project of mine is to practice classifying human non-speech audio using a 1D CNN. The model processes MFCC features extracted from each audio file and classifies them into categories like breath, cough, laugh, and more. 


Model performance so far:


Validation set accuracy: 79.57%


Test set accuracy: 64.55%


The model performs well on distinct classes like breath and laugh but struggles with crying with cough, laugh, and screaming. Sneeze and yawn are also challenging, likely due to fewer samples and overlapping sound patterns.



## Dataset
I got the dataset from: [Nonspeech7k dataset](https://zenodo.org/records/6967442) (Rashid et al., 2023), containing 7,014 strongly labeled 32 kHz mono .wav files across 7 classes, which is used for this project.

The original authors [Classification and analysis of human non-speech sounds](https://ietresearch.onlinelibrary.wiley.com/doi/am-pdf/10.1049/sil2.12233) achieved:

79% accuracy with a 12-layer CNN on raw waveforms (M12 model)


~65–70% accuracy with baseline MFCC+CNN models

