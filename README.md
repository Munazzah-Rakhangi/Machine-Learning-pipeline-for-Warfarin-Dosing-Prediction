💊 **Machine Learning Pipeline for Warfarin Dose Prediction**

📌 Project Overview
This project focuses on building a machine learning pipeline to predict the therapeutic Warfarin dose for patients. 
Warfarin is widely prescribed as an anticoagulant, but dosing is challenging due to high inter-patient variability 
and its narrow therapeutic index. Incorrect dosing can lead to severe bleeding or clotting events, making accurate 
dose prediction critical for patient safety.

To address this, I applied multiple supervised learning models to the International Warfarin Pharmacogenetics 
Consortium (IWPC) dataset. The pipeline covers data preprocessing, model training, evaluation, and comparison, 
with the aim of identifying the most reliable model for dose prediction and supporting the personalization of 
anticoagulant therapy.

------------------------------------------------------------

📂 **Dataset**
- Source: PharmGKB – International Warfarin Pharmacogenetics Consortium (IWPC)  
- Description: The dataset contains patient-level demographic, clinical, and genetic information relevant to Warfarin dosing.  
- Key Features:  
  - Demographics (age, weight, height, race/ethnicity)  
  - Clinical factors (target INR, enzyme inhibitors)  
  - Genetic variants (CYP2C9, VKORC1)  

------------------------------------------------------------

🤖 **Models Implemented**
We experimented with the following machine learning models:

- K-Nearest Neighbors (KNN)  
- Random Forest Regressor (RF)  
- Support Vector Regression (SVR)  
- Feed-Forward Neural Network (FFNN)  

Each model was trained and evaluated using a consistent preprocessing pipeline to ensure fair comparison.

------------------------------------------------------------

📊 **Model Performance**
Evaluation was conducted using Mean Absolute Error (MAE), Mean Squared Error (MSE), and the R² score.

| Model                          | MAE   | MSE   | R² Score |
|--------------------------------|-------|-------|----------|
| K-Nearest Neighbors (KNN)      | 5.18  | 47.96 | 0.59     |
| Random Forest (RF)             | 4.82  | 41.87 | 0.64     |
| Support Vector Regression (SVR)| 5.49  | 51.44 | 0.55     |
| Feed-Forward Neural Network    | 4.39  | 38.72 | 0.68     |

Best Model: The Feed-Forward Neural Network (FFNN) achieved the lowest error and highest R², showing the 
greatest potential for accurate Warfarin dose prediction.

------------------------------------------------------------

⚙️ **Tech Stack**
- Language: Python  
- Libraries: scikit-learn, pandas, numpy, matplotlib, seaborn, TensorFlow/Keras  
- Environment: Jupyter Notebook / VS Code  

------------------------------------------------------------

🚀 **How to Run**
1. Clone this repository:
   git clone https://github.com/Munazzah-Rakhangi/Machine-Learning-pipeline-for-Warfarin-Dosing-Prediction.git
   cd Machine-Learning-pipeline-for-Warfarin-Dosing-Prediction

2. Install required dependencies:
   pip install -r requirements.txt

3. Open the notebook:
   jupyter notebook Warfarin_Dose_Prediction.ipynb

4. Run all cells to reproduce the results.

------------------------------------------------------------

⭐ **Acknowledgments**
- International Warfarin Pharmacogenetics Consortium (IWPC) for providing the dataset.  
- PharmGKB for maintaining open pharmacogenomics data resources.  
- Inspiration drawn from the critical importance of personalized medicine in clinical practice.  

------------------------------------------------------------

✨ If you find this project useful, please give it a star on GitHub and share it with others interested in AI for healthcare.
