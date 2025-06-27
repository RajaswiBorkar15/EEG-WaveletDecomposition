# EEG-WaveletDecomposition
This project aims to **classify EEG signals** as either **depressed (MEC)** or **healthy (HEC)** by leveraging **discrete wavelet transform (DWT)** for feature extraction and multiple **machine learning models** for classification.

## Project Workflow
1. **Load EEG data** using `MNE` from `.edf` files
2. **Denoise EEG signals** via wavelet thresholding
3. Perform **2-level or 5-level wavelet decomposition** (depending on wavelet)
4. Extract subbands: Delta, Theta, Alpha, Beta, Gamma
5. Compute **statistical + nonlinear features**:
 - Mean, Std, Median, IQR, Skewness, Kurtosis, Coefficient of Variation, Energy
 - Approximate Entropy (ApEn), Sample Entropy (SampEn)
6. Perform **ANOVA-based feature selection**
7. Train **10 ML classifiers**:
 - Random Forest, SVM, KNN, XGBoost, LightGBM, Naive Bayes, Decision Tree, Logistic Regression, MLP, Extra Trees
8. **Evaluate and compare** model performance using accuracy scores
9. **Visualize** accuracy table and trends across wavelets
   
## Tech Stack
- Python, NumPy, Pandas, Matplotlib, Seaborn
- MNE for EEG signal loading
- PyWavelets (`pywt`) for wavelet transformation
- Antropy for entropy features
- Scikit-learn, XGBoost, LightGBM
