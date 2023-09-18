![image](https://github.com/ad451/BatteryModelling/assets/71942892/f7e962fa-5fde-4ea3-82c8-919e293d7fcb)# Battery Modeling Jupyter Notebook

## Overview

This repository contains a Jupyter notebook that demonstrates battery modeling using the SPMT (Single Particle Model with Thermal effects) approach. The notebook focuses on the following aspects:

- Calculating the Open Circuit Voltage (OCV) using the SPMT model.
- Obtaining experimental OCV vs. State of Charge (SOC) data from the Marquis2019 dataset in PyBaMM.
- Simulating battery discharge under various conditions, including constant C-rates (0.1 to 10) and time-varying current profiles (e.g., sinusoidal).
- Calculating errors between the SPMT-modeled OCV and experimental OCV.
- Developing a simple neural network-based residual model to predict errors and improve OCV estimation.
- Evaluating model performance using Root Mean Square Error (RMSE) and Relative Error Ratio (RER).

## Notebook Usage

1. **Data Preparation**: The notebook provides step-by-step instructions on loading and preprocessing experimental OCV vs. SOC data.

2. **Constant C-rate Modeling**:
   - Run the relevant cells to train the SPMT model for constant C-rates and calculate errors.
   - Evaluate model performance using RMSE and RER.

3. **Time-Varying Current Modeling**:
   - Simulate battery discharge using time-varying current profiles, e.g., sin(2πt/60).
   - Calculate errors for the SPMT model.
   - Observe how varying current affects model performance.

## Notebook Contents

- `battery_modeling.ipynb`: The Jupyter notebook containing code, explanations, and visualizations for battery modeling.|

## Performance

- ### Constant Current Case
[![image.png](https://i.postimg.cc/xC213j46/image.png)](https://postimg.cc/xk6Q0QYm)

- ### Varying Current Case
[![image.png](https://i.postimg.cc/xdS2Wx3C/image.png)](https://postimg.cc/LJvwPV7K)

## Graphs
[![image.png](https://i.postimg.cc/XND0V7kt/image.png)](https://postimg.cc/V5MhgwTF)

[![image.png](https://i.postimg.cc/cH9P4Xwf/image.png)](https://postimg.cc/WFZ55m94)

## Acknowledgments

- This project utilizes the PyBaMM library for battery modeling. PyBaMM is an open-source project, and we acknowledge the PyBaMM community for providing valuable tools and resources. For more information, visit the [PyBaMM GitHub repository](https://github.com/pybamm-team/PyBaMM).

- We also acknowledge the scikit-learn library for its contributions to machine learning and neural network modeling in this project. Scikit-learn is an essential part of our work. For more information, visit the [scikit-learn website](https://scikit-learn.org/stable/index.html).

Feel free to customize this README and the notebook as needed to provide more details about the notebook's content, usage, and any specific instructions for users.
