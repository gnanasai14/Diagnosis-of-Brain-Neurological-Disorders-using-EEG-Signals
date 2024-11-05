# Detection of brain neurological disorders with Electroencephalogram signals using Random Forest classifier comparing with Linear Discriminant Analysis classifier

R. Gnanasai
Research Scholar,
Department of Electronics and Communication Engineering, 
Saveetha School of Engineering,
Saveetha Institute of Medical and Technical Sciences, 
Saveetha University, Chennai, Tamil Nadu, India. Pincode:602105
rallapallignanasai17@saveetha.com


K. Vidhya
Project Guide, Corresponding Author,
Department of Electronics and Communication Engineering, 
Saveetha School of Engineering,
Saveetha Institute of Medical and Technical Sciences, 
Saveetha University, Chennai, Tamil Nadu, India. Pincode:602105
vidhyak.sse@saveetha.com


Abstract. The aim of the study is to improve the accuracy, recall, precision and specificity in detecting brain neurological disorders with Electroencephalogram (EEG) signals using Random Forest (RF) algorithm in comparison with Linear Discriminant Analysis (LDA). Using RF and LDA, EEG recordings representing the brain activity of 20 samples in each group are identified as epileptic or non-epileptic. The novelty in this study is selection of prominent features from EEGs using the concept of mutual information.  The RF algorithm yielded accuracy (95.85 %), recall (91.33 %), precision (88.28 %), and specificity (96.99 %), whereas the LDA approach yielded accuracy (68.84 %), recall (42.21 %), precision (31.43 %), and specificity (76.33 %).  The difference between the two groups is significant, since p0.05. RF classifiers are significantly more accurate in detecting neurological disorders in the brain than LDA classifiers.


Keywords: Electroencephalogram (EEG) signals, Epilepsy, Novel Feature, Signal Processing, Random Forest (RF), Linear Discriminant Analysis (LDA).

INTRODUCTION


There may be about 1% of the world's population who suffer from epilepsy. Seizure detection is crucial for epilepsy patients since epilepsy impacts their psychological and physical interactions. Monitoring brain activity with electroencephalograms (EEG) has become the standard approach to epilepsy diagnosis.  Epileptic signals can be captured using EEG signals and seizure status can be determined using EEG signals. EEG signals can detect interictal and ictal epileptic variations between seizures. In order to spot pre-ictal spikes and patterns of seizures, trained neurologists use visual inspection to interpret EEG readings. The evaluations given by an EEG are used to make sure or rule out varied conditions, including autism, alzheimer, epilepsy disorder. The researchers proposed an self-regulated method to encounter epileptic seizure from EEG signals and the accomplishment is calculated in terms of accuracy, precision, specificity and sensitivity. A process that involves a trained neurophysiologist to inspect the EEG signals manually, that are used to diagnose epilepsy. As a result, a self-regulating method is needed to analyze the EEG signal and diagnose epilepsy.

Le Douget used Discrete Wavelet Transform (DWT) for feature extraction allowing a multiresolution analysis of the signal. Gulnur Tolebi presented a method that classifies signals into three classes, seizure free, pre-seizure and seizure. With the help of raw EEG data and data under different noise levels were evaluated. Recognition accuracy is better, but it needs to be improved. Yol Seyma proposed the Empirical Mode Decomposition (EMD) technique, with which the highest accuracy (96.97%) is obtained. It has been observed that the proposed method can be used for classifying healthy data and epileptic data. Prabhakar used the Eigenvector technique with Pisarenko’s method for feature extraction. The optimized values are finally classified using Decision Trees, Random Forest (RF) and Linear Discriminant Analysis (LDA) classifiers. Using RF classifiers, the highest classification accuracy (95.57%) is obtained. Previously our team has a rich experience in working on various research projects across multiple disciplines.

The drawback of the existing system is that to provide the right predictions, a large number of decision trees are employed. The aim of the study is to boost the accuracy of diagnosing brain neurological disorders using EEG signals with RF classifiers by determining the one with the most votes would be chosen from among the available output classes, and due to that, reliable execution would be ensured.

MATERIALS AND METHODS

The study was carried out in the Department of Electronics and Communication Engineering at Saveetha School of Engineering, Saveetha Institute of Medical And Technical Sciences, Chennai. There are two groups namely, RF and LDA. The total sample size is 40 and pretest power for the sample size is 80%. 

The sample preparation for group 1 RF, comprises 20 EEG signals collected from the UCI database.  The samples are preprocessed by filtering and removing artifacts using notch filters and  further processed.

The sample preparation for group 2 LDA, comprises EEG signals collected from the UCI database.  The samples are preprocessed by filtering and removing artifacts using notch filters and  further processed.On the UCI machine learning repository, the EEG signal dataset is convenient (online open-source). The dataset consists of 500 patients and 4097 EEG measurements taken every 23.5 seconds from each patient. The 4097 data points were then separated into 23 blocks, each block consisting of 178 data points for 1 second displayed in one row in the dataset, and these blocks were distributed evenly among the patients. There are 178 readings in each and every row, or, put another way, 178 data points for every second. Totally, there are 11,500 rows of data and 179 columns with the last column containing the status of the patient, whether the patient is having an epileptic seizure or not.

For the execution of these algorithms utilizing signal processing techniques, the Google Colaboratory software and the Python programming tool are installed in a system with a Ryzen 7 CPU and 8GB RAM memory. Entropy and energy characteristics are calculated using EEG data.  The important novel features from the derived novel features are selected using mutual information based on entropy. Random Forest is a common and efficient supervised machine learning algorithm that can perform both regression and classification tasks. The Random Forest Classifier can be used both in image processing and signal processing techniques. The Random Forest Classifier class is imported using the Sklearn Ensemble library. In the training  process, these features are fed into the Random forest model with labeling (1 for abnormal and 0 for normal). Random Forest algorithms are a type of ensemble learning algorithm that uses a training dataset to create a number of decision trees that can predict test results. When training data is fed into the decision tree's input, a set of rules is created. These rules are then applied to test data in order to predict the class of new instances. Random forests generate a forest of decision tree models, each one based on a random sample of training data. Unlike decision trees, which consider all features when constructing a model, these algorithms generate each decision tree using a random sample of features from the feature space. Test data can be run through each of these trees to collect votes.

It is first necessary to create a function based on the function that maximizes the differences between groups. Similarly, the second function maximizes the difference in the previous function without being correlated with it. For the following functions, it is essential that none of the previous functions be correlated with the new function. LDA works when the calculations made on independent variables for each observation are continuous quantities. Analyzing discriminant correspondence is the equivalent technique, when handling categorical independent variables.

Statistical Analysis

SPSS is used to perform statistical analysis [24]. Age, gender, and epilepsy duration are independent factors, while accuracy, recall, precision, and specificity are dependent variables. Algorithm performance is compared using an independent t-test. The proposed work uses Google Colaboratory to diagnose brain neurological disorders using  RF and LDA classifiers and signal processing techniques.

RESULTS

The suggested RF (95.85%, 91.33%, 88.28% and 96.99% respectively) performs much better than LDA (68.84%, 42.21%, 31.43% and 76.33%  respectively) in terms of accuracy, recall, precision, and specificity. In RF, 0.05 standard deviation and 0.00 standard error are measured after statistical analysis of 20 samples, but in LDA, 0.02 standard deviation and 0.00 standard error are measured after statistical analysis of 20 samples.

The value of p (Sig.(2-tailed)) is 0.000, which is less than 0.05. Hence, it is concluded that the results obtained by the classification are very much significant. 

From the results obtained, the performance of the RF algorithm is comparatively better than the LDA method.

DISCUSSION

The Random Forest algorithm was outstandingly greater than the Linear Discriminant Analysis classifier with an accuracy of 95.85% using signal processing techniques. The execution of Random Forest and LDA algorithms are analyzed in diagnosing the brain neurological disorders from EEG signals (normal and abnormal) and the samples were gathered from UCI machine learning repository (online open-source). The selection of prominent novel features from EEGs is executed using the idea of mutual information. The advised work shows that the Random Forest algorithm has a significantly better detection rate compared to LDA.

The RF classifier yields an average accuracy of 98% in diagnosing neurological disorders if  depression diagnosis index is calculated automatically based on EEG recordings. The RF classification performance in terms of accuracy, sensitivity and specificity can be improved if complexity-based novel features are considered (accuracy of 97%). RF is achieving higher performance with an accuracy of 94.5%, because it uses structural risk minimization principle. The RF classification performance can be improved with appropriate random state value. 

 The multiple function kernel provides better performance (accuracy of 89.24%). compared with SVM based on a single function kernel(accuracy of 81.61%). Septiarini proved that Multi Layer Perceptron (MLP) with accuracy of 94% is comparatively better in diagnosing brain disorders than RF with an accuracy of 92.9%. Classification accuracy of 97.72% is obtained with Naive Bayes Classifier using soft computing Techniques.
The limitation of this study was the Random forest algorithm can make a large number of classes which might cause slowness to the algorithm. In future, adding more novel features and by increasing the number of EEG signals would certainly improve the detection rate using the Random forest algorithm. This work can also be used to improve the performance of real-time applications.

CONCLUSION 

The performance of Random Forest classifiers in determining epileptic seizure is comparatively better than Linear Discriminant Analysis. The execution of the proposed system is tested in respect of accuracy, recall, precision and specificity using EEG recordings of the patients. The average accuracy, recall, precision and specificity  obtained using Random Forest classifier (95.85%, 91.33%, 88.28% and 96.99% respectively) is comparatively greater than Linear Discriminant Analysis classifier (68.84%, 42.21%, 31.43% and 76.33% respectively). The classification is executed with EEG signals using signal processing techniques.
