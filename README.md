# Parkinson's Disease Detection using Machine Learning

## Project Description
This project aims to detect Parkinson's Disease using voice features. Parkinson's Disease is a neurodegenerative disorder that affects movement, and early detection can significantly improve the quality of life for patients. This machine learning model uses a **Random Forest Classifier** to predict whether a person has Parkinson's Disease based on their voice features.

The dataset used in this project contains voice recordings from healthy individuals and those with Parkinson's Disease. The dataset includes **23 features** extracted from each voice recording, such as fundamental frequency, jitter, shimmer, and harmonic-to-noise ratio.

---

## Dataset
The dataset contains **195 voice recordings** with **24 features** extracted from each recording. The features include measures such as:
- **MDVP:Fo(Hz)**: Average vocal fundamental frequency
- **MDVP:Fhi(Hz)**: Maximum vocal fundamental frequency
- **MDVP:Flo(Hz)**: Minimum vocal fundamental frequency
- **MDVP:Jitter(%)**, **MDVP:Jitter(Abs)**, **MDVP:RAP**, **MDVP:PPQ**, **Jitter:DDP**: Measures of variation in fundamental frequency
- **MDVP:Shimmer**, **MDVP:Shimmer(dB)**, **Shimmer:APQ3**, **Shimmer:APQ5**, **MDVP:APQ**, **Shimmer:DDA**: Measures of variation in amplitude
- **NHR**, **HNR**: Noise-to-Harmonics Ratio and Harmonics-to-Noise Ratio
- **RPDE**, **DFA**, **spread1**, **spread2**, **D2**, **PPE**: Nonlinear dynamic complexity measures
- **status**: Target variable (0 = healthy, 1 = Parkinson's Disease)

The dataset is provided below:

```csv
name,MDVP:Fo(Hz),MDVP:Fhi(Hz),MDVP:Flo(Hz),MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP,MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:APQ,Shimmer:DDA,NHR,HNR,RPDE,DFA,spread1,spread2,D2,PPE,status
phon_R01_S01_1,119.992,157.302,74.997,0.00784,0.00007,0.0037,0.00554,0.01109,0.04374,0.426,0.02182,0.0313,0.02971,0.06545,0.02211,21.033,0.414783,0.815285,-4.813031,0.266482,2.301442,0.284654,1
phon_R01_S01_2,122.4,148.65,113.819,0.00968,0.00008,0.00465,0.00696,0.01394,0.06134,0.626,0.03134,0.04518,0.04368,0.09403,0.01929,19.085,0.458359,0.819521,-4.075192,0.33559,2.486855,0.368674,1
phon_R01_S01_3,116.682,131.111,111.555,0.0105,0.00009,0.00544,0.00781,0.01633,0.05233,0.482,0.02757,0.03858,0.0359,0.0827,0.01309,20.651,0.429895,0.825288,-4.443179,0.311173,2.342259,0.332634,1
phon_R01_S01_4,116.199,141.17,78.63,0.00989,0.00008,0.00493,0.0064,0.0148,0.04774,0.457,0.02459,0.03498,0.03237,0.07376,0.01353,20.644,0.434969,0.819235,-4.117501,0.334147,2.405554,0.368975,1
phon_R01_S01_5,116.199,141.17,78.63,0.00989,0.00008,0.00493,0.0064,0.0148,0.04774,0.457,0.02459,0.03498,0.03237,0.07376,0.01353,20.644,0.434969,0.819235,-4.117501,0.334147,2.405554,0.368975,1
