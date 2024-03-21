# Earthquake Prediction using Machine Learning

## Project Overview
This project focuses on predicting the magnitude of earthquakes using a dataset called "Earthquake.csv." The dataset contains several features related to earthquake events, and the goal is to predict the magnitude of these events. 
## Dataset Description

The "Earthquake.csv" dataset comprises the following columns:

1. **Latitude**: The geographical latitude where the earthquake occurred. Latitude can influence the proximity of populated areas to the earthquake epicenter and can be correlated with earthquake magnitude.

2. **Longitude**: The geographical longitude where the earthquake occurred. Longitude provides information about the geographic location of the earthquake, which can be relevant for predicting magnitude, as seismic activity varies by region.

3. **Depth**: The depth at which the earthquake originated beneath the Earth's surface. Deeper earthquakes may have different magnitudes and effects compared to shallow ones, making depth an important predictor.

4. **MagType**: The type of magnitude measurement used (e.g., Richter scale, moment magnitude scale). Different magnitude types have distinct mathematical formulations, and choosing the appropriate one is crucial for accurate prediction.

5. **Nst**: The total number of earthquake stations used to determine magnitude. A higher number of stations can contribute to more accurate magnitude estimation.

6. **Gap**: The largest azimuthal gap between earthquake stations contributing to magnitude determination. A large gap might introduce uncertainty in magnitude estimation.

7. **RMS**: The root mean square of the amplitude spectrum of the earthquake's seismic signal. RMS provides information about the seismic waveform, which can be used to estimate magnitude accurately.

8. **MagNst**: The total number of stations reporting the magnitude. A larger number of reporting stations can lead to more precise magnitude estimates.

9. **Mag**: The target variable we aim to predict, representing the magnitude of the earthquake.

## How these fields affects magnitude of an earthquake

- **Latitude and Longitude**: These geographical coordinates can be used to determine the location of the earthquake epicenter. Certain regions are more prone to larger earthquakes, so latitude and longitude can indirectly influence magnitude predictions.

- **Depth**: Deeper earthquakes often result in higher magnitudes. Depth can be directly correlated with magnitude, as deeper earthquakes tend to release more energy.

- **MagType**: The choice of magnitude type affects the mathematical formula used for magnitude estimation. The type of magnitude can significantly impact the predicted magnitude.

- **Nst, Gap, and MagNst**: These columns provide information about the number and distribution of earthquake stations reporting data. More stations and smaller gaps between them can contribute to more accurate magnitude estimates.

- **RMS**: The root mean square of the seismic signal can provide insights into the amplitude and frequency characteristics of the earthquake, which are factors used in magnitude estimation.

## Project Significance

Earthquake prediction is a critical area of research with significant implications for public safety and infrastructure resilience. Accurate earthquake magnitude prediction can help:

- **Early warning systems:** Provide advance warning to affected areas, potentially saving lives and minimizing damage.

- **Infrastructure planning:** Inform building codes and infrastructure design to withstand earthquakes of various magnitudes.

- **Disaster response:** Allocate resources effectively based on expected earthquake magnitude and impact.

## Machine Learning Models

To predict earthquake magnitudes, three machine learning models were employed:

1. **Regression Model (Linear Regression)**: Linear regression is a simple model used as a baseline for prediction. It establishes a linear relationship between features and magnitude.

2. **Artificial Neural Network (ANN)**: A neural network model designed to capture complex non-linear relationships between features and magnitude.

3. **Random Forest**: A decision tree-based ensemble model that combines multiple decision trees for improved prediction accuracy.

## Model Accuracy

The accuracy of the models was evaluated, and the results are as follows:

- ANN (Artificial Neural Network) achieved the highest accuracy among the three models.

- Random Forest performed better than Linear Regression, indicating its ability to capture non-linear patterns in the data.

## Visualization

Geopandas is used to create geographical plots of earthquake data. The varying earthquake magnitudes are visually represented, helping us understand the distribution of earthquake magnitudes across different locations.
![image](https://github.com/Vageesh-Jayaraman/Earthquake-Prediction/assets/143870355/4f775df8-467b-41f0-8d6d-b16bff57a6e6)

## Conclusion
This project demonstrates the potential of machine learning in earthquake magnitude prediction, which can contribute to early warning systems and informed decision-making for disaster management and infrastructure planning. The use of Geopandas for visualization adds an important spatial dimension to the analysis.

