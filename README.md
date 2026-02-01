# 🧬 Alzheimer's Drug Discovery with Machine Learning

This project employs Machine Learning (Random Forest) to predict the bioactivity of chemical compounds targeting the **Acetylcholinesterase (AChE)** enzyme, a key target for Alzheimer's disease treatment.

## 🚀 Project Overview
- **Goal:** Predict the **pIC50** value (potency) of a molecule based on its chemical structure.
- **Data Source:** ChEMBL Database (Bioactivity data for AChE).
- **Algorithm:** Random Forest Regressor.
- **Descriptors:** Morgan Fingerprints (ECFP4) generated via RDKit.

## 📊 Performance
The model achieved an **R² score of 0.75**, successfully distinguishing between active Alzheimer's drugs (e.g., Donepezil) and inactive compounds.

## 🛠️ Technologies Used
- Python
- RDKit (Cheminformatics)
- Scikit-learn (Machine Learning)
- Pandas & Matplotlib

## 👨‍💻 How to Run
Click the "Open in Colab" badge above to run the notebook directly in your browser.
