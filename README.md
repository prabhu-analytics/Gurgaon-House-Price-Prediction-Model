# Gurgaon-House-Price-Prediction-Model
🏡 Gurgaon House Price Prediction
This project builds a machine learning pipeline to predict house prices in Gurgaon using the California housing dataset as a proxy. It includes data preprocessing, model training, and inference, with the pipeline and model saved for production-ready deployment.
📌 Project Overview
- Goal: Estimate Gurgaon house prices using a proxy dataset.
- Dataset: California Housing dataset (housing.csv)
- Model: Random Forest Regressor
- Deployment: Pipeline and model saved using Joblib for efficient reuse.
🧰 Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Joblib
⚙️ How It Works
🔧 Training Phase
- Reads housing.csv
- Creates income categories for stratified sampling
- Splits data using StratifiedShuffleSplit
- Preprocesses features:
- Numerical: imputation + scaling
- Categorical: one-hot encoding
- Trains a RandomForestRegressor
- Saves the trained model and pipeline as model.pkl and pipeline.pkl
🔍 Inference Phase
- Loads saved model and pipeline
- Reads new input data from input.csv
- Applies preprocessing and generates predictions
📁 File Structure
├── housing.csv          # Training dataset
├── input.csv            # New data for prediction
├── output.csv           # Prediction results
├── model.pkl            # Trained model
├── pipeline.pkl         # Preprocessing pipeline
├── main.py              # Main script (code provided above)
├── README.md            # Project documentation

📊 Output
- Predictions are added to input.csv as a new column: median_house_value
- Final results saved in output.csv
🔮 Future Enhancements
- Replace proxy dataset with actual Gurgaon housing data
- Add support for multiple models and hyperparameter tuning
- Build a web interface for real-time predictions


- Saves results to output.csv

