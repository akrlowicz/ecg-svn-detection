# ecg-svn-detection
Classifying supraventricular and ventricular peaks in ecg recording. 

# Data
Using MIT-BIH Suprvaentricular Arrythmia Database https://physionet.org/content/svdb/1.0.0/ containg 78 half-hour ECG recordings chosen to supplement the examples of supraventricular arrhythmias in the MIT-BIH Arrhythmia Database.
Important note: loading database to dict is performed with private function that I did not include in repository. 

# Classification
Supraventricular beats are characterized by long time interval between peaks. Ventricular peaks can be irregular and disturbed. 
It's important to distinguish between those peaks and normal ones, especially when they look similar. This was the aim of the project.
The problem is complex, because of the data (results from MIT db didn't apply to real-world data + classes are highly imbalanced) and nature of the problem (peaks can be similar, supraventicular class was praticulary hard to classify). 
Tried SVM, XGBoost, LD, SMOTE and Bledning methods.
Didn't achieve great results, nevertheless learned a lot of things about ECG signal.

# Literature
1. "Detection of supraventricular and ventricular ectopic beats using a single lead ECG", Philip De Chazal, IEEE, 2013, URL: https://ieeexplore.ieee.org/document/6609433
2. "Heartbeat Classification Using Normalized RR Intervals and Morphological Features", Chun-Cheng Lin and Chun-Min Yang, Mathematical Problems in Egineering, 2014, URL: https://www.hindawi.com/journals/mpe/2014/712474/
