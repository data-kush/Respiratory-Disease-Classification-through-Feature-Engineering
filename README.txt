Respiratory Disease Classification through Feature Engineering
Introduction
This initiative centers on classifying respiratory conditions using advanced feature engineering and machine learning methods. It employs data augmentation, SMOTE (Synthetic Minority Oversampling Technique), a Convolutional Neural Network (CNN) model, and Mel-frequency cepstral coefficients (MFCC) features to enhance disease identification. The objective is to conduct binary classification for individual respiratory conditions and multi-class classification for broader analysis.
Project Summary
Respiratory illnesses pose a major public health challenge, and timely diagnosis is vital for effective intervention. This project focuses on identifying respiratory conditions from audio recordings using sophisticated computational techniques.
Data Augmentation
To enrich the training dataset's variety, data augmentation techniques are implemented, including:

Adding random noise
Time-stretching
Pitch modulation

SMOTE for Addressing Class Imbalance
To mitigate class imbalance within the dataset, SMOTE is utilized to oversample underrepresented classes, ensuring a balanced distribution.
Convolutional Neural Network (CNN)
A CNN model is adopted due to its proficiency in extracting spatial patterns from MFCC representations of audio data.
Mel-frequency Cepstral Coefficients (MFCC)
MFCC features are derived from audio recordings, offering a concise and effective representation for audio-based classification tasks.
Dataset Description
The ICBHI 2017 Respiratory Sound Database, initially developed for a scientific challenge, is used in this project. The current version, combining public and private datasets, is openly accessible for research. It comprises 920 audio recordings from 126 patients, totaling 5.5 hours and including 6898 breathing cycles. Of these, 886 cycles contain wheezes, 1864 contain crackles, and 506 include both. Respiratory experts annotated the cycles for the presence of wheezes, crackles, or no adventitious sounds. Recordings, ranging from 10 to 90 seconds, were captured using various devices and include chest location details.
Each filename consists of five elements:

Recording index
Patient ID (101, 102, ..., 226)
Chest location:
Lateral right (Lr)
Lateral left (Ll)
Posterior right (Pr)
Trachea (Tc)
Anterior left (Al)
Anterior right (Ar)
Posterior left (Pl)


Recording device:
WelchAllyn Meditron Master Elite Electronic Stethoscope (Meditron)
3M Littmann 3200 Electronic Stethoscope (Litt3200)
3M Littmann Classic II SE Stethoscope (LittC2SE)
AKG C417L Microphone (AKG C417L)


Acquisition mode:
Simultaneous/multichannel (mc)
Sequential/single channel (sc)



The dataset includes four columns:

Presence/absence of wheezes (1 = present, 0 = absent)
Presence/absence of crackles (1 = present, 0 = absent)
Start of respiratory cycle(s)
End of respiratory cycle(s)

Abbreviations used:

LRTI (Lower Respiratory Tract Infection)
COPD (Chronic Obstructive Pulmonary Disease)
URTI (Upper Respiratory Tract Infection)

Results
The project reports outcomes for binary and multi-class classification, including metrics such as accuracy, precision, recall, sensitivity, specificity, and F1-score. Visualizations, such as confusion matrices, may be included to illustrate performance.