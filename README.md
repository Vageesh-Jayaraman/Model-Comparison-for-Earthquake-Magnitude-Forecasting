# Earthquake Magnitude Prediction Model Evaluation

## Project Overview
This project focuses on evaluating the performance of machine learning algorithms in predicting the magnitude of earthquakes using a dataset called "Earthquake.csv." While the primary objective is not earthquake prediction itself, but rather the comparison of different algorithms for magnitude estimation.

## Dataset Description

The "Earthquake.csv" dataset comprises the following columns:

1. **Latitude**: The geographical latitude where the earthquake occurred.
2. **Longitude**: The geographical longitude where the earthquake occurred.
3. **Depth**: The depth at which the earthquake originated beneath the Earth's surface.
4. **MagType**: The type of magnitude measurement used.
5. **Nst**: The total number of earthquake stations used to determine magnitude.
6. **Gap**: The largest azimuthal gap between earthquake stations contributing to magnitude determination.
7. **RMS**: The root mean square of the amplitude spectrum of the earthquake's seismic signal.
8. **MagNst**: The total number of stations reporting the magnitude.
9. **Mag**: The target variable representing the magnitude of the earthquake.

## Evaluation of Model Performance

- **Regression Model (Linear Regression)**: Utilized as a baseline for prediction. Establishes a linear relationship between features and magnitude.
- **Artificial Neural Network (ANN)**: Designed to capture complex non-linear relationships between features and magnitude.
- **Random Forest**: An ensemble model combining multiple decision trees for improved prediction accuracy.

## Model Accuracy Assessment

- ANN achieved the highest accuracy among the three models.
- Random Forest outperformed Linear Regression, indicating its ability to capture non-linear patterns in the data.

## Visualization

Geopandas is used to create geographical plots of earthquake data. The varying earthquake magnitudes are visually represented, aiding in understanding the distribution of earthquake magnitudes across different locations.

![Earthquake Magnitude Distribution](https://github.com/Vageesh-Jayaraman/Earthquake-Prediction/assets/143870355/4f775df8-467b-41f0-8d6d-b16bff57a6e6)

## Conclusion
While the primary focus of this project is not on earthquake prediction, the evaluation of machine learning algorithms for earthquake magnitude estimation holds significance. The findings contribute to understanding the comparative effectiveness of different models, which can inform future research directions and practical applications in early warning systems, disaster management, and infrastructure planning. The use of Geopandas for visualization adds a crucial spatial dimension to the analysis.
