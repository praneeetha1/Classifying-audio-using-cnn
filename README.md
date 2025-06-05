# Audio_classifier_cnn  
A 1D CNN model for classifying human non-speech audio into 7 categories: breath, cough, crying, laugh, screaming, sneeze, and yawn. The model processes MFCC features extracted from audio files.

## Model Performance  
- **Validation accuracy**: 79.57%  
- **Test accuracy**: 64.55%  

The model performs reliably on distinct classes like **breath** and **laugh**, but shows confusion between:  
- **Crying** ↔ cough/laugh/screaming  
- **Sneeze** ↔ breath/crying  
- **Yawn** ↔ breath  

These challenges likely stem from overlapping acoustic features and class imbalance in training data.

## Dataset  
[Nonspeech7k dataset](https://zenodo.org/records/6967442) (Rashid et al., 2023)  
- 7,014 labeled 32 kHz mono .wav files  
- 7 non-speech classes  

## Related Research  
The original authors achieved:  
- **79% test accuracy** using a 12-layer CNN on raw waveforms ([Classification and analysis of human non-speech sounds](https://ietresearch.onlinelibrary.wiley.com/doi/10.1049/sil2.12233))  
- **~65–70% accuracy** with baseline MFCC+CNN architectures  

This project recreates their MFCC baseline approach with comparable results, demonstrating the viability of simpler models for this task. Future work will explore deeper architectures and raw waveform processing.



~65–70% accuracy with baseline MFCC+CNN models

