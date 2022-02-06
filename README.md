# Cardiac-Disease-Prediction
This an open source project that detects the possibility of cardiac diseases using Bayesian Networks. The application consists of two parts (Graphical user interface (GUI), backend). The GUI has been created with the QT designer tool and more specifically, the framework Pyqt5 that enables the user to interact with the application through impressive graphics and functions. Backend reads a dataset containing 14 variables for each patient about various factors that affect the possibility of cardiac disease. Dataset reading is done by using Python where the csv file is read line by line to create a training model in Problog.This dataset contains 76 attributes, but all published experiments refer to using a subset of 14 of them.I found the dataset at (https://www.kaggle.com/ronitf/heart-disease-uci) and the creators of these database (https://archive.ics.uci.edu/ml/datasets/Heart+Disease) are:

    Hungarian Institute of Cardiology. Budapest: Andras Janosi, M.D.
    University Hospital, Zurich, Switzerland: William Steinbrunn, M.D.
    University Hospital, Basel, Switzerland: Matthias Pfisterer, M.D.
    V.A. Medical Center, Long Beach, and Cleveland Clinic Foundation: Robert Detrano, M.D., Ph.D.
    
In total, 14 variables are contained for each patient and the variables are:

    1. Age
    2. Gender
    3. Chest pain type
    4. Resting blood pressure
    5. Serum cholesterol
    6. Fasting blood sugar
    7. Resting electrocardiographic results
    8. Maximum heart rate
    9. Exercise
    10. ST depression
    11. The slope of the peak exercise ST segment
    12. Number of major vessels colored by fluoroscopy
    13. Thalassemia
    14. Target

Then the application reads the data given by the user to calculate the possibility of cardiac disease and display the result using the Problog. Problog language calculates the possibility of cardiac diseases using Bayesian Networks.

Example:
If we assume that a twenty-three man with the following variables:

    1. Age in years (1-100): 23
    2. Gender (1 = male; 0 = female): 1
    3. Chest pain type (4 values: 0-3): 1
    4. Fasting blood sugar 120 mg/dl (1 = true; 0 = false): 0
    5. Resting blood pressure (1-200): 146
    6. Serum cholestoral in mg/dl (1-400): 245
    7. Exercise induced angina (1 = yes; 0 = no): 1
    8. Resting electrocardiographic results (0,1,2): 0
    9. Maximum heart rate achieved (1-300): 123
    10. Number of major vessels (0-3) colored by flourosopy: 0
    11. ST depression induced by exercise relative to rest (0-3): 0
    12. Slope of the peak exercise ST segment (0-2): 1
    13. Thalassemia (1= normal; 3 = reversable defect): 4
    
The probability of occur cardiac disease this man is 0.4562 as shown in below Figure.

![image](https://user-images.githubusercontent.com/57871380/152681116-b9e6f70c-a20f-4d77-92f1-7333c2d62655.png)


The project was based on the following research from which I extracted a lot of information:

    Nikos Papatheodorou, Nikos Ntantinakis, Stefanos Zervoudakis, Emmanouil Marakakis, and Haridimos Kondylakis. 2020. A Probabilistic Logic Program that Predicts COVID-19 Infection and the Possibility a Patient to Recover. In 24th Pan-Hellenic Conference on Informatics (PCI 2020). Association for Computing Machinery, New York, NY, USA, 272–276. DOI:https://doi.org/10.1145/3437120.3437323

- Attention: The above application was created as part of a course for practicing programming languages. It is not used for medical purposes as there is a high probability of invalid results and the only purpose of its creation is to practice programming.

Personal info:

    Developer: Anastasios Koumarelis (akoumarelis@gmail.com)
    University: Hellenic Mediteranian University, Department of Electrical and Computer Engineering, Msc in Informatics Engineering
    Course: Advanced Topics In Artificial Intelligence 2020-2021
