### Fault-Diagnosis-of-Electric-drives-using-ML

AC Electric Drives, commonly referred to as Variable Speed Drives (VSDs), are extensively used across industrial, domestic, and commercial applications due to their capability to deliver desired torque, power levels, and control for various external load requirements. The Three Phase Induction Motor is often utilized in these drives because of its simplicity and durability. However, the drive components, particularly the induction motor, are prone to faults, leading to costly maintenance, downtime, and potential safety risks.

### Project Overview

This project aims to perform time-series analysis on critical and non-critical faults, encompassing both electrical and mechanical issues. Using statistical feature extraction techniques, the project identifies information-rich regions from motor output data. This is followed by Machine Learning-based multi-class classification to accurately identify various faults, ensuring high accuracy and quick diagnosis for timely corrective measures.

#### Key Objectives:
1. **Data Generation**: A Variable Frequency Drive model was simulated using Simulink in MATLAB.
2. **Fault Simulation**: Five specific faults were chosen and simulated:
   - Under Voltage Fault
   - Over Voltage Fault
   - Phase to Ground Short Circuit Fault
   - Phase to Phase Short Circuit Fault
   - Over Loading Fault
   These faults, along with normal operating conditions, form the six target categories for prediction.

### Data Preparation

#### Data Generation and Transformation
- Data was collected under multiple loading conditions, relative to full load torque.
- The raw signal/waveform data was converted into data matrices and stored in CSV files.

#### Feature Selection
Six output parameters/features were selected for further analysis.

#### Data Preprocessing Steps:
1. **Steady-state Data Segregation**
2. **Data Imputation**
3. **Label Encoding**
4. **Feature Scaling**
5. **Data Shuffling**

### Model Building

Three supervised machine learning models were chosen for the multi-class classification task:
1. **K-Nearest Neighbor (KNN)**
2. **Support Vector Machine (SVM)**
3. **Random Forest**

These models were trained using K-fold cross-validation and optimized using grid search for hyperparameter tuning.

### Model Evaluation

The models' performance was evaluated using various metrics:
- **Accuracy**
- **Confusion Matrix**
- **Training Time**

Results indicated that the K-Nearest Neighbor model outperformed the others, achieving a classification accuracy of 93.13% on the testing set.

### Conclusion

The project demonstrated the efficacy of machine learning in diagnosing faults in AC electric drives. The high classification accuracy and comprehensive evaluation of multiple algorithms provided a robust methodology for fault diagnosis. This study highlights the potential of machine learning in motor conditioning and response generation, opening avenues for further exploration in this emerging field.

By comparing multiple supervised classification algorithms, the project provided a thorough understanding of the best-performing models, contributing to the advancement of fault diagnosis techniques in the industry. The methodology developed offers a reliable and accurate solution for fault diagnosis in AC electric drives used in various sectors.
