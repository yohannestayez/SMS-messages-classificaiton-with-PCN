# SMS spam Classification Report
## Overview
In this mini project, I used the **ngclearn** library to design, implement, and train a **Predictive Coding Network (PCN)** for classifying SMS messages as spam or non-spam. This approach is inspired by **neural processing principles**. The data was preprocessed and trough an architecture with two hidden layers, the PCN was trained on the preprocessed SMS dataset using Hebbian learning mechanisms. Details of the notebook include:
1.	**Data loading**
    - Imported and loaded SMS data into pandas dataframe
2.	**Data Cleaning**
    - Renamed the columns as label and messages
    - Removed duplicate rows if any
    - Removed special characters, numbers, punctuations and extra spaces and converted all the texts to lowercase. 
    - Eliminated unimportant words.
3.	**EDA**
    - Analyzed class distribution
    - Visualized word frequency, common keyword, and message length
4.	**Data preprocessing**
    - Encoded spam and ham labels as 1 and 0 respectively
    - Added new column (message length) showing the length of each text
5.	**Feature Extraction**
    - Used **TF-IDF** to transform text data into numerical feature matrices
6.	**Model Architecture Design**
    - Built a **Predictive coding network (PCN)** with input, 2 hidden layers and an output layer using the **ngclearn** library. 
    - Each cell defined by **Ratecell** nodes, and error signal by **Errorcell** nodes.
    - Synaptic connection established for generative(forward) and error(backward) pathways.
7.	**Model Training**
    - PCN model was trained using **Hebbian learning framework**.
    - Weights updated iteratively to minimize prediction errors.
    - Conducted training over 30 epochs with a batch size of 32 to optimize the model parameters.

8.	**Evaluation**
    - Evaluation conducted on the test dataset. Results show excellent results showing results with all metrics being around 97.29%

    


