# EEG-WaveletDecompsiton
This project focuses on classifying EEG signals using wavelet feature extraction followed by machine learning classifiers such as SVM, Random Forest, and Gradient Boosting. The EEG signals are processed using 3-level discrete wavelet decomposition, and statistical features are extracted from subbands to build accurate classification models.
## Project Highlights
- EEG signal preprocessing and denoising
- 3-level **Wavelet Decomposition with Different Wavelets**
- Feature extraction from wavelet coefficients
- **StandardScaler**, **PCA**, and **SelectKBest** for dimensionality reduction
- Trained multiple classifiers: SVM, Random Forest, Gradient Boosting and others
- Evaluated with accuracy, classification report, and confusion matrix
## Tech Stack
- Python
- NumPy, OpenCV, PyWavelets
- Scikit-learn, Matplotlib, Seaborn
