# Machine Learning for Age Detection

This repository contains a machine learning project for predicting a person's age based on their voice. Multiple audio features are extracted from each input file, and various machine learning models are trained to predict the age. The best-performing model is selected based on evaluation metrics.

## Features Extracted from Audio Files

The following audio features are extracted to aid in age prediction:

- **Mel-frequency cepstral coefficients (MFCCs)**
- **Chroma feature**
- **Spectral contrast**
- **Zero-crossing rate**
- **Spectral rolloff**
- **Root mean square error**

Additionally, the following statistical features are calculated:

- **Spectrogram**: Mean and standard deviation
- **Spectral bandwidth**: Mean and standard deviation
- **Spectral contrast**: Mean and standard deviation
- **Spectral flatness**: Mean and standard deviation
- **Spectral rolloff**: Mean and standard deviation
- **Chroma features**: Mean and standard deviation
- **MFCC**: Mean and standard deviation
- **Delta MFCCs**: First and second derivatives (mean and standard deviation)
- **Frequency statistics**: Mean, standard deviation, skewness, and kurtosis

## Models Used

This project evaluates the performance of several machine learning algorithms, including:

- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **MLP Regressor**
- **Support Vector Regressor (SVR)**
- **Random Forest Regressor**
- **Decision Tree Regressor**
- **RANSAC Regressor**
- **Huber Regressor**
- **Gradient Boosting Regressor**
- **HistGradientBoosting Regressor**

### Hyperparameter Tuning

Each model is trained using a grid of hyperparameters. The following parameters are tuned:

- **LinearRegression**: `fit_intercept`
- **Ridge**: `alpha`, `solver`
- **Lasso**: `alpha`, `solver`
- **MLPRegressor**: `hidden_layer_sizes`, `activation`, `alpha`, `learning_rate`, `max_iter`
- **SVR**: `C`, `epsilon`, `kernel`, `gamma`
- **RandomForestRegressor**: `n_estimators`, `max_depth`, `min_samples_split`, `max_features`
- **DecisionTreeRegressor**: `max_depth`, `min_samples_split`, `min_samples_leaf`, `max_features`
- **RANSACRegressor**: `estimator`, `min_samples`, `residual_threshold`, `max_trials`
- **HuberRegressor**: `epsilon`, `alpha`, `max_iter`, `tol`, `fit_intercept`
- **GradientBoostingRegressor**: `n_estimators`, `learning_rate`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `max_features`, `subsample`, `loss`
- **HistGradientBoostingRegressor**: Similar to `GradientBoostingRegressor`

The best performing model is the selected.