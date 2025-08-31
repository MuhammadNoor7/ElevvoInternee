1️⃣ Student Classification & Score Prediction

Objective: Predict student exam performance based on study patterns and background variables.

🔹 Steps

Data Loading & Preprocessing

Imported dataset using Pandas & NumPy.

Handled missing values.

Applied ordinal encoding for categorical features and binary encoding for gender, extracurriculars, internet access, and learning disabilities.

Exploratory Data Analysis (EDA)

Visualized relationships such as Hours Studied vs Exam Score.

Modeling

Linear Regression (Hours only).

Polynomial Regression (Degree 2).

Multivariate Linear Regression.

Evaluation Metrics

MAE, MSE, RMSE, R², Adjusted R².

📌 Key Learnings

✔ Regression modeling fundamentals.
✔ Feature selection impact.
✔ Interpreting evaluation metrics.
✔ Effect of multiple variables on student outcomes.

2️⃣ Forest Cover Type Classification

Objective: Classify forest cover type based on environmental and topographical variables.

🔹 Steps

Data Preprocessing

Handled missing values (mean for numeric, mode for categorical).

Dropped low-variance columns.

Applied ordinal encoding.

EDA

Histograms & KDE plots for feature distributions.

Correlation heatmap for numeric + encoded features.

Modeling

Random Forest Classifier.

XGBoost Classifier (with label encoding).

Hyperparameter tuning using RandomizedSearchCV.

Visualized representative decision trees for interpretability.

📌 Key Learnings

✔ Multi-class classification.
✔ Data preprocessing techniques.
✔ Hyperparameter tuning.
✔ Feature importance & interpretability in tree-based models.

3️⃣ Music Data Analysis

Objective: Classify music genres using audio features, MFCCs, and spectrograms.

🔹 Steps

Data Handling

Imported multiple datasets (3s/30s features, MFCCs, spectrograms).

Cleaned missing values, dropped low-variance columns.

Applied ordinal encoding for categorical features.

EDA

Visualized feature distributions (tempo, loudness, energy).

Correlation heatmaps & class balance analysis.

Feature Engineering

Extracted MFCCs from audio files.

Prepared & augmented spectrograms (resizing, normalization, rotations, shifts, flips).

Modeling

Random Forest & XGBoost (tabular features).

Custom CNN (Conv2D, MaxPooling2D, Dense, Dropout, Flatten).

Transfer Learning with VGG16 & ResNet50.

Optimized training with EarlyStopping & ReduceLROnPlateau.

📌 Key Learnings

✔ Audio feature extraction & MFCC processing.
✔ CNN design & transfer learning.
✔ Spectrogram-based classification.
✔ Regularization & callbacks for stable training.

4️⃣ Walmart Sales Prediction

Objective: Predict Walmart weekly sales using historical, seasonal, and economic data.

🔹 Steps

Data Preparation

Merged datasets (train, test, stores, features).

Converted Date to datetime & sorted chronologically.

Handled missing values, dropped low-variance columns.

EDA

Boxplots, scatterplots, pairplots, correlation heatmaps.

Feature Engineering

Time features: year, month, week, dayofweek.

Seasonal flags: spring, summer, fall, winter.

Store attributes: holiday encoding, store type, store size bins.

Lag features (lag_1, lag_4, lag_40).

Rolling means (10, 20).

Delta features (Fuel_Price_Change, CPI_Change).

Interaction features (Temp_Fuel_Interaction).

Final Dataset Size: 294,513 rows × 40 columns.

Modeling

Random Forest.

Linear Regression.

XGBoost.

LightGBM.

Best Model: XGBoost (RMSE ≈ 4194, MAE ≈ 1660, R² ≈ 0.968).

📌 Key Learnings

✔ Large-scale feature engineering.
✔ Time-series forecasting.
✔ Ensemble methods for business predictions.
✔ Model comparison using regression metrics.

⚙️ Tech Stack & Tools
🛠 Languages & Libraries

Python

NumPy, Pandas

Matplotlib, Seaborn

Statsmodels

Librosa

🤖 Machine Learning Frameworks

scikit-learn (StandardScaler, OrdinalEncoder, LabelEncoder, RandomizedSearchCV)

Models: RandomForestClassifier, XGBoost, LightGBM

🧠 Deep Learning (TensorFlow/Keras)

Sequential API

Conv2D, MaxPooling2D, Dense, Dropout, Flatten, GlobalAveragePooling2D

VGG16, ResNet50 (Transfer Learning)

ImageDataGenerator (augmentation)

EarlyStopping, ReduceLROnPlateau

📚 Concepts Covered

Regression & Classification

Feature Engineering (tabular, audio, image, time-series)

CNNs & Transfer Learning

Hyperparameter Tuning

Model Evaluation & Metrics

Time-Series Forecasting
