# DF-VLS: Distance-Free Visible Light Sensing for Indoor Localization

## Overview

DF-VLS (Distance-Free Visible Light Sensing) is an indoor localization framework that estimates user positions using Visible Light Communication (VLC) signals without relying on conventional RSS-to-distance conversion methods.

The project investigates machine learning-based localization techniques by directly mapping received signal characteristics to spatial coordinates, improving robustness against non-linear channel effects and environmental variations.

---

## Features

* Indoor VLC channel modeling
* RSS data generation from multiple LED Access Points
* Distance-Free localization approach
* Machine Learning based position estimation
* Random Forest localization baseline
* Performance evaluation using localization error metrics
* Visualization of user positions and predicted locations

---

## System Model

The simulation environment consists of:

* Room Dimensions: 5 m × 5 m × 3 m
* Multiple VLC Access Points mounted on the ceiling
* Randomly distributed users
* Lambertian optical channel model
* Photodiode-based receiver

The framework generates RSS measurements from visible light sources and uses machine learning algorithms to predict user coordinates directly.

---

## Repository Structure

```text
DF-VLS/
│
├── data/                 # Generated datasets
├── figures/              # Plots and visualizations
├── models/               # Trained ML models
├── notebooks/            # Jupyter notebooks
├── src/                  # Source code
│   ├── channel_model.py
│   ├── dataset_generator.py
│   ├── localization.py
│   └── random_forest.py
│
├── results/              # Experimental results
├── main.py               # Main execution script
├── requirements.txt
└── README.md
```

---

## Methodology

1. Generate user locations inside the room.
2. Compute RSS values from VLC Access Points.
3. Construct localization dataset.
4. Train Random Forest regression model.
5. Predict user coordinates.
6. Evaluate localization performance using positioning error.

---

## Evaluation Metrics

* Mean Absolute Error (MAE)
* Root Mean Square Error (RMSE)
* Average Localization Error
* Cumulative Distribution Function (CDF) of localization error

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/DF-VLS.git
cd DF-VLS
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Run the localization framework:

```bash
python main.py
```

Or open the Jupyter notebook:

```bash
jupyter notebook
```

---

## Results

The proposed DF-VLS framework demonstrates accurate indoor localization by directly learning the relationship between VLC signal features and user positions, eliminating the need for explicit distance estimation.

Future work includes:

* XGBoost-based localization
* Deep Neural Networks
* Hybrid VLC-THz localization
* Mobility-aware localization
* OIRS-assisted VLC systems

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-Learn
* Matplotlib
* Jupyter Notebook

---

## Author

**Govind Kumar Jha**

B.Tech Electronics and Communication Engineering

Research Internship – AI for Wireless Systems

IIIT Delhi

---

## License

This project is intended for academic and research purposes.
