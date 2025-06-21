# Network Traffic Anomaly Detection for Telecom Security

This project provides a production-grade, telecom-focused workflow for detecting anomalies in network traffic using both unsupervised and supervised machine learning. It leverages the NSL-KDD dataset, advanced feature engineering, and models optimized for telecom environments.

## Features
- Telecom-specific feature engineering (5G core-aware)
- Unsupervised anomaly detection (Isolation Forest)
- Supervised classification (Random Forest, XGBoost)
- Business impact analysis and compliance notes
- Ready for cloud/edge deployment

## Installation

1. **Clone the repository or download the project files.**

2. **Install dependencies:**

   It is recommended to use a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. **(Optional) Install Jupyter Notebook:**
   ```bash
   pip install notebook
   ```

## Usage

1. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open `network_traffic_anomaly_detection.ipynb` in your browser.**

3. **Run all cells in order:**
   - The notebook will download the NSL-KDD dataset automatically.
   - It will preprocess, engineer features, train models, and display results.

4. **Model Deployment:**
   - Trained models and scaler are saved as `.joblib` files for production use.
   - Example inference code is provided in the notebook.

## Project Structure
- `network_traffic_anomaly_detection.ipynb` — Main notebook with all code and documentation
- `requirements.txt` — List of required Python packages
- `README.md` — This file
- `nokia_ml_data/` — Downloaded dataset files
- `nokia_rf_security_model.joblib`, `nokia_xgb_security_model.joblib`, `nokia_scaler.joblib` — Saved models/scaler (after running the notebook)

## Notes
- The workflow is designed for telecom/5G security use cases but can be adapted to other domains.
- All features are anonymized and GDPR-compliant.
- For best results, use the latest versions of Python 3.8+ and all listed packages.

## Troubleshooting
- If you encounter import errors, ensure all packages in `requirements.txt` are installed.
- For issues with Jupyter, try restarting the kernel and running all cells again.

## License
This project is provided for educational and demonstration purposes.
