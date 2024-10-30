# Inner_Speech_Prediction
The project aimed to classify raw EEG signals into categories. It includes real-time EEG signal processing, data cleaning using techniques like ICA, and building DL models to classify inner thoughts into their class.

**Project Overview**
This project leverages real-time EEG data from human subjects, processed to clean and analyze neural signals, and then applied deep learning techniques to convert these signals into spoken language. Using a combination of advanced filtering techniques and neural networks, the system captures the neural patterns related to inner speech and translates them into speech output.

**Data Collection**
                        Subjects: 10 subjects from different age groups.
                        Equipment: Neophony headband (8 channels).
                        Channels: Captured electrical activity from different brain regions.
                        
**Preprocessing**
                        Library Used: MNE for loading, filtering, and processing EEG data from EDF files.
                        Artifact Removal: ICA (Independent Component Analysis) to clean eye movements and muscle activity.
                        Notch Filtering: Applied to remove 50Hz noise from electrical signals.
                        
**Model Development**
                        Model Used: LSTM for classifying EEG signals into speech.
                        Accuracy: Achieved approximately 70% accuracy after fine-tuning.
                        Outcome: Good results considering available resources and equipment.
