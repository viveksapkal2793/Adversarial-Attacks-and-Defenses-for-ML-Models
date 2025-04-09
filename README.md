# Adversarial Machine Learning: Analysis, Attacks & Defenses

## Project Overview

This project explores the vulnerability of machine learning models to adversarial examples and implements various defense strategies to enhance model robustness. Through a series of Jupyter notebooks, we demonstrate model evaluation, adversarial attack implementation, and defense mechanism development using the IAPRTC-12 dataset.

## Notebooks Description

1. **`task_0.ipynb`**: Model Evaluation and Baseline Performance
   - Implements and evaluates multiple machine learning algorithms
   - Performs feature engineering and hyperparameter tuning
   - Establishes baseline performance metrics

2. **`task_1.ipynb`**: Adversarial Attack Implementation and Analysis
   - Implements various adversarial attack methodologies (FGSM, PGD)
   - Analyzes attack success rates across different models
   - Visualizes the impact of perturbation magnitude on attack effectiveness

3. **`task_2.ipynb`**: Defense Mechanisms and Robustness Enhancement
   - Implements four defense strategies: adversarial training, defensive preprocessing, robust ensemble, and adversarial detection
   - Evaluates and compares defense effectiveness
   - Analyzes trade-offs between robustness and clean accuracy

## Installation and Setup

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook environment

### Required Libraries

```
numpy>=1.20.0
scipy>=1.7.0
scikit-learn>=1.0.0
pandas>=1.3.0
matplotlib>=3.4.0
seaborn>=0.11.0
joblib>=1.0.0
tqdm>=4.60.0
```

### Installation Steps

1. Clone the repository:
   ```
   git clone https://github.com/viveksapkal2793/Adversarial-Attacks-and-Defenses-for-ML-Models
   ```

2. Create and activate a virtual environment (recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use: venv\Scripts\activate
   ```

3. Install required packages:
   ```
   pip install numpy scipy scikit-learn pandas matplotlib seaborn joblib tqdm
   ```

## Dataset Setup

This project uses the IAPRTC-12 image classification dataset.

1. Download the IAPRTC-12 dataset from [the official website](http://www.iapr-tc12.org/)
2. Create a directory named IAPRTC within the project folder
3. Place the following files in the IAPRTC directory:
   - `IAPRTC-12_TrainFeat.mat`
   - `IAPRTC-12_TrainLabels.mat`
   - `IAPRTC-12_TestFeat.mat`
   - `IAPRTC-12_TestLabels.mat`

## Directory Structure

```
assign_2/
│
├── task_0.ipynb              # Model evaluation notebook
├── task_1.ipynb              # Adversarial attack notebook
├── task_2.ipynb              # Defense strategies notebook
├── README.md                 # This file
│
├── IAPRTC/                   # Dataset directory
│   ├── IAPRTC-12_TrainFeat.mat
│   ├── IAPRTC-12_TrainLabels.mat
│   ├── IAPRTC-12_TestFeat.mat
│   └── IAPRTC-12_TestLabels.mat
│
├── models/                   # Created during execution, stores trained models
├── adversarial_examples/     # Created during execution, stores attack examples
├── defense_comparison_plots/ # Created during execution, stores visualization results
└── various defense results   # Multiple directories created during defense evaluation
```

## Execution Instructions

1. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

2. Open and execute the notebooks in sequence:
   - Start with task_0.ipynb to establish baseline models
   - Proceed to task_1.ipynb to implement and analyze attacks
   - Finally, run task_2.ipynb to implement and evaluate defenses

3. Each notebook contains markdown cells explaining the concepts and code implementation. Execute cells sequentially (Shift+Enter) to ensure dependencies are properly established.

## Additional Notes

- Saved models and intermediate results will be stored in automatically created directories
- The notebooks generate various visualizations comparing model performance, attack effectiveness, and defense capabilities
- Some cells may take significant time to execute, particularly those involving model training and adversarial example generation
- Memory requirements may be substantial when processing the entire dataset
