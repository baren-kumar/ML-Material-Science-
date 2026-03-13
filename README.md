Composite Material Property Prediction using Gaussian Process Regression
Overview


This project demonstrates how Machine Learning can be used to predict the mechanical strength of carbon fiber–epoxy composite materials using Gaussian Process Regression (GPR).
The model learns the relationship between composite composition parameters and the resulting material strength, enabling fast prediction and surrogate modeling for composite material design.
This work is useful for researchers and students working in materials science, composite engineering, and machine learning–based material design.
________________________________________
Project Objectives
•	Predict composite tensile strength using Machine Learning
•	Apply Gaussian Process Regression (GPR) for material property prediction
•	Demonstrate uncertainty estimation in predictions
•	Provide a simple ML workflow for composite material datasets
________________________________________
Dataset
The dataset contains 500 simulated composite material samples.
Input Features
•	carbon_fiber_fraction – fraction of carbon fiber in the composite
•	epoxy_resin_fraction – fraction of epoxy matrix
•	volume_fraction – fiber volume fraction
Target Output
•	strength – predicted tensile strength of the composite (MPa)
Example dataset format:
carbon_fiber_fraction	epoxy_resin_fraction	volume_fraction	strength
0.55	0.45	0.60	820
0.60	0.40	0.65	900
0.50	0.50	0.55	780
________________________________________
Methodology
The workflow used in this project:
1.	Load composite dataset
2.	Preprocess data using feature scaling
3.	Split dataset into training and testing sets
4.	Train a Gaussian Process Regression (GPR) model
5.	Predict composite strength
6.	Evaluate model performance
7.	Estimate prediction uncertainty
Workflow diagram:
Dataset → Preprocessing → Train GPR Model → Prediction → Evaluation
________________________________________
Machine Learning Model
The project uses Gaussian Process Regression (GPR) with the following kernel structure:
•	Constant Kernel
•	Radial Basis Function (RBF) Kernel
•	White Kernel (noise component)
This kernel combination allows the model to capture nonlinear relationships between composite parameters and material strength.
________________________________________

________________________________________

________________________________________
Usage
Run the Jupyter notebook:
jupyter notebook Comp_GPR.ipynb
The notebook will:
•	Load the composite dataset
•	Train the Gaussian Process model
•	Predict material strength
•	Display prediction uncertainty
•	Visualize model performance
________________________________________
Example Prediction
Input parameters:
•	Carbon fiber fraction = 0.60
•	Epoxy resin fraction = 0.40
•	Fiber volume fraction = 0.65
Model output:
Predicted Strength ≈ 920 MPa
Prediction Uncertainty ≈ ±10 MPa
________________________________________
Applications
This approach can be applied to:
•	Composite material design
•	Surrogate modeling for FEA simulations
•	Materials informatics research
•	Machine learning–based material discovery
•	Mechanical property prediction
________________________________________
