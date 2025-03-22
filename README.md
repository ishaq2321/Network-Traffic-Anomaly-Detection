# Network Traffic Anomaly Detection

## Overview
This project demonstrates how to detect anomalies in network traffic data using both unsupervised and supervised machine learning techniques. The workflow covers data acquisition, preprocessing, feature engineering, model training, evaluation, and reporting. The project is highly relevant for cybersecurity and network monitoring applications.

## Dataset
- **NSL-KDD**: A widely used benchmark dataset for network intrusion detection, containing labeled network traffic records with normal and attack types.
- Downloaded directly in the notebook from public sources.

## Project Structure
- `network_traffic_anomaly_detection.ipynb`: Main Jupyter notebook with the complete workflow and explanations.
- `plan.md`: Project planning and phase breakdown.
- `requirements.txt`: List of required Python packages.
- `data/`: Directory where the NSL-KDD dataset files are stored after download.

## Workflow
1. **Data Acquisition**
   - Download and load the NSL-KDD dataset.
2. **Data Preprocessing & Exploration**
   - Handle missing values, encode categorical features, normalize numerical features.
   - Perform exploratory data analysis (EDA) with visualizations.
3. **Feature Engineering**
   - Remove highly correlated features.
   - Optionally create new features (e.g., bytes ratio).
   - Apply PCA for dimensionality reduction and visualization.
4. **Unsupervised Anomaly Detection**
   - Use Isolation Forest and DBSCAN to detect anomalies without labels.
   - Visualize results in PCA space and evaluate using available labels.
5. **Supervised Classification**
   - Train a Random Forest classifier using labeled data.
   - Evaluate with precision, recall, F1-score, confusion matrix, and ROC curve.
6. **Model Evaluation & Visualization**
   - Summarize and compare the performance of all models.
   - Discuss strengths and limitations.
7. **Documentation & Reporting**
   - Summarize the project, findings, and next steps.

## Key Findings
- Unsupervised models (Isolation Forest, DBSCAN) can detect anomalies without labels but may have lower precision/recall.
- Supervised models (Random Forest) generally achieve higher accuracy when labeled data is available.
- Feature engineering and data preprocessing are critical for both approaches.
- Visualizations (PCA, confusion matrix, ROC curve) help interpret model performance and data separability.

## How to Run
1. Clone the repository or copy the project folder.
2. (Recommended) Create and activate a Python virtual environment:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open `network_traffic_anomaly_detection.ipynb` in Jupyter or VS Code and run all cells in order.

## Next Steps
- Experiment with additional algorithms (e.g., SVM, XGBoost).
- Tune hyperparameters for improved performance.
- Deploy the model for real-time anomaly detection.
- Extend the notebook with more advanced visualizations and reporting.


---

**End of README**
