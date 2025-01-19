# EEG Seizure Classification and Explainability Model

This project focuses on classifying EEG (Electroencephalogram) signals into different seizure types while incorporating explainability techniques to build clinical trust. The objective is to create a robust, interpretable model to assist neurologists in diagnosing and managing neurological disorders.

## Problem Statement

The task involves the classification of EEG signals into four classes:
1. **Normal** (Non-seizure EEGs)
2. **Complex Partial Seizures**
3. **Electrographic Seizures**
4. **Video-detected Seizures with no visual change over EEG**

The solution must also integrate explainability techniques to identify critical EEG channels influencing the classification.

### Key Objectives:
- Process time-domain and frequency-domain EEG signals to extract features.
- Train baseline and advanced models for classification.
- Implement xAI techniques for interpretability.
- Denoise noisy EEG data to improve performance.
- Use generative models to augment datasets with synthetic EEG data.

---

## Project Workflow

1. **Data Preprocessing and Visualization**:
   - Visualize raw EEG signals for all 19 channels.
   - Compute basic metrics like mean, variance, energy, etc.

2. **Feature Extraction**:
   - Extract frequency-domain features using Fourier Transform and Wavelet Decomposition.
   - Analyze spectrograms for time-frequency characteristics.

3. **Baseline Model**:
   - Train a Support Vector Machine (SVM) using Fourier features and Zero Crossing Rates.
   - Evaluate using classification reports and ROC-AUC scores.

4. **Advanced Modeling**:
   - Optimize features and hyperparameters.
   - Experiment with advanced techniques, including deep learning.

5. **Explainability**:
   - Use SHAP or saliency maps to identify critical EEG channels.
   - Analyze the impact of these channels on model predictions.

6. **Denoising**:
   - Apply signal denoising techniques and report PSNR.
   - Evaluate performance on cleaned data.

7. **Synthetic Data Generation**:
   - Generate synthetic EEG signals using generative algorithms.
   - Train models on synthetic data and evaluate against real data-trained models.

---

## Evaluation Criteria

Performance is evaluated based on:
- Classification accuracy, ROC-AUC scores, and balanced accuracy.
- Model efficiency (minimal parameters).
- Explainability and impact of critical EEG channels.

---

## Tools and Libraries

- **Languages**: Python
- **Libraries**: 
  - Data Analysis: `NumPy`, `Pandas`
  - Visualization: `Matplotlib`, `Seaborn`
  - Machine Learning: `Scikit-learn`
  - Signal Processing: `PyWavelets`
  - Explainability: `SHAP`
  - Advanced Modeling: `TensorFlow` or `PyTorch` (optional)

---

## Submission Guidelines

1. Include all code in a GitHub repository or Jupyter Notebook.
2. Document your approach in a README file or markdown cells.
3. Submit the `test_outputs.csv` file for evaluation.

---

## Acknowledgments

This project is part of the **Impulse 2025 Hackathon** on Biomedical Signal Processing.
