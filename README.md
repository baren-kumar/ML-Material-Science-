
Forward and Inverse Machine Learning Approaches for Composite Material Property Prediction and Manufacturing Process Analysis

Project Overview

This repository presents a Machine Learning framework for composite material design, combining Forward Modeling and Inverse Modeling to predict material properties and optimize manufacturing parameters.
The project demonstrates how machine learning can be integrated with simulation datasets (e.g., FEA) to enable rapid prediction of composite mechanical properties and guide the design of new composite materials.

The framework focuses on predicting properties such as:

•	Tensile Strengt

•	Elastic Modulus

•	Failure Stress

•	Process–property relationships

This repository is intended for researchers in composite materials, materials informatics, and computational materials engineering.
________________________________________
Research Objectives

The main objectives of this project are:

•	Develop forward ML models for predicting composite properties from material composition and manufacturing parameters.

•	Develop inverse ML models for identifying optimal material parameters given target properties.

•	Demonstrate surrogate modeling for simulation-based composite design.

•	Enable data-driven composite material discovery.
________________________________________

Methodology

Forward Machine Learning Model

The forward model predicts material properties from input parameters.
Inputs
•	Fiber type

•	Fiber volume fraction

•	Matrix properties

•	Fiber orientation

•	Cure temperature

•	Manufacturing pressurs

Outputs

•	Tensile strength

•	Elastic modulus

•	Failure strain

Workflow:

Material Composition + Process Parameters
                ↓
        Forward ML Mode
           ↓
        Predicted Properties
        
________________________________________

Inverse Machine Learning Model

The inverse model determines the optimal material parameters required to achieve target properties.
Inputs

•	Target tensile strength

•	Target elastic modulus

Outputs

•	Fiber volume fraction

•	Resin composition

•	Manufacturing parameters



Workflow:

Target Properties
        ↓     
    Inverse Model
       ↓
Recommended Material Design

________________________________________

Machine Learning Models Used

Several machine learning models are implemented for material property prediction:

•	Gaussian Process Regression (GPR)

•	Random Forest

•	Support Vector Regression (SVR)

•	Artificial Neural Networks (ANN)

•	Gradient Boosting (XGBoost)

These models are used to construct surrogate models for fast prediction compared to computationally expensive simulations.


Dataset

The dataset contains composite material samples generated from:

•	experimental studies

•	finite element simulations

•	literature datasets

Typical dataset features include:

Feature	Description

fiber_type	Carbon / Glass

fiber_volume_fraction	Fiber percentage

matrix_type	Polymer matrix

orientation	Fiber orientation angle

curing_temperature	Manufacturing temperature

pressure	Processing pressure


Target properties:
•	Tensile Strength

•	Elastic Modulus

•	Failure Strain




Applications

This framework can be applied to:

•	Composite material design

•	Surrogate modeling for FEA simulations

•	Materials informatics

•	Data-driven material discovery

•	Manufacturing process optimization



Author

Baren Kumar Baidya

Master’s in Data Science & Machine Learning

B.Sc in Mechanical Engineering 




