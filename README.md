# Predictive Maintenance for CNC Machines - Project Overview
This repository contains a Streamlit web application that leverages a deep learning model to predict potential failures in CNC machines. Predictive maintenance is a critical component of Industry 4.0, helping industries prevent costly downtime and improve operational efficiency. By analyzing key operational parameters, the app predicts the type of failure, enabling timely corrective actions.
# Workflow of the Project
# Data Collection:

Data was collected from CNC machine sensors, capturing parameters such as air temperature, process temperature, rotational speed, torque, tool wear, and job type.
# Data Preprocessing:

Feature scaling was applied using a Scikit-learn scaler (scaler.pkl) to standardize the input parameters.
# Model Training:

A deep learning model was developed using Keras.
The model architecture included layers with custom activation functions like LeakyReLU.
The model was trained to classify six possible outcomes: five failure types and a "No Failure" scenario.
# Saving the Model:

The trained model was saved in HDF5 format (model1_ip.h5), ensuring compatibility with TensorFlow for deployment.
# Streamlit Application Development:

A user-friendly interface was developed in Streamlit to accept user inputs for key operational parameters:
Job Type (Low, Medium, High)
Air Temperature
Process Temperature
Rotational Speed
Torque
Tool Wear
Input features are preprocessed using the loaded scaler, and predictions are made using the trained model.
# Prediction:

The application predicts the class of failure and displays a descriptive status to the user, helping them take preventive measures.
# Deployment and Sharing:

The project is packaged for easy sharing via GitHub, ensuring reproducibility and scalability
