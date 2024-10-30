# Inner_Speech_Prediction
The project aimed to classify raw EEG signals into categories. It includes real-time EEG signal processing, data cleaning using techniques like ICA, and building DL models to classify inner thoughts into their class.
**Converting Thoughts/Inner Speech to Speech**
This project focuses on translating neural signals, specifically inner thoughts or inner speech, into spoken language using EEG data. The goal is to explore advanced neural signal processing techniques and deep learning models to create a system that converts EEG signals into speech.

**Project Overview**
This project leverages real-time EEG data from human subjects, processed to clean and analyze neural signals, and then applied deep learning techniques to convert these signals into spoken language. Using a combination of advanced filtering techniques and neural networks, the system captures the neural patterns related to inner speech and translates them into speech output.

**Data Collection**
We collected raw EEG signals from 10 subjects of different age groups using the Neophony headband(8 channels).EEG signals were recorded using multiple channels(8), which correspond to the electrodes placed on different parts of the subject’s scalp. Each channel captures electrical activity from a specific region of the brain, helping in isolating and analyzing different neural patterns related to inner speech. The data was recorded using the Neophony app, which provided two types of data files:
        EDF: Used for storing bio-signal data, particularly useful for signal processing and analysis.
        CSV: Easier for handling and basic data analysis tasks.
        
**Preprocessing**
To ensure clean and usable data, we applied several preprocessing techniques to remove noise and unwanted artifacts
MNE liberary was used to load, filter, and manipulate EEG data, from EDF files. ICA was employed to separate and remove artifacts such as eye movements and muscle activity from the EEG data. Nnoch-filtering was applied to stable 50Hz pick due to electric signals.

**Model Development**
The cleaned EEG data was used to develop deep learning models to translate neural signals into speech.
After preprocessing, the data was structured into suitable input formats for the model.
A LSTM model was used for classification, after fine tuning we reached an accuracy around 70% we is considered sufficiently good considering the resources and equipments that were available.

