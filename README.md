# Lithology Classification Using Deep Neural Networks

This repository demonstrates the application of **Deep Neural Networks (DNNs)** for lithology classification using geophysical parameters such as Vp, Density, and Poisson’s Ratio (PR). The project is divided into two notebooks: binary classification (shale vs. sand) and multi-class classification (shale, sand, hydrocarbon sand). The results highlight the capability of DNNs to classify lithology without explicit reliance on rock physics models.

---

## [Notebook 1: Binary Lithology Classification](https://github.com/yjliu212/Lithology-Classification-Using-Deep-Neural-Network/blob/main/Assignment_3_Lithology_Classification_Prediction.ipynb)

### Objective:
Classify lithology into two classes:
- **0:** Shale
- **1:** Sand  

### Methodology:
1. **Dataset Generation**  
   - Vp, Density, and PR were randomly sampled within predefined ranges to simulate realistic geophysical data.  
   - The dataset was labeled using a rock physics model to distinguish shale from sand.  
   - **Training/Test Split**: 80% for training, 20% for testing.  

   **Sampled Data Points**:
   ![Sample Data Distribution](https://github.com/user-attachments/assets/f2cedcbc-f850-407c-8f1a-44ff6e770fb2)

2. **Model Training**  
   - A DNN model was trained for 10 epochs to learn the relationship between the input features and lithology classification.  

   **Training Data with Classes (0 = Shale, 1 = Sand)**:
   ![Training Dataset](https://github.com/user-attachments/assets/60928499-5656-4b68-8af7-ef1d397b5fec)

3. **Results**  
   - The trained DNN successfully captured the underlying pattern and separated shale and sand in the test dataset:  
     ![Testing Results](https://github.com/user-attachments/assets/4c3a348d-f1c0-4144-94b1-7a115d4ca59c)  

   - **Prediction Confidence**: The model output included probabilities for each prediction, highlighting the uncertainty associated with the classification:  
     ![Prediction Confidence](https://github.com/user-attachments/assets/af4b25a8-c109-4759-9689-698b7589a395)

---

## [Notebook 2: Multi-class Lithology Classification](https://github.com/yjliu212/Lithology-Classification-Using-Deep-Neural-Network/blob/main/Assignment_3b_Lithology_Multi_Classification_Prediction.ipynb)

### Objective:
Extend the classification to three lithology classes:
- **0:** Shale  
- **1:** Sand  
- **2:** Hydrocarbon Sand (HC Sand)

### Methodology:
1. **Dataset Generation**  
   - Added a new class (HC Sand) to the existing dataset, increasing the complexity of the classification task.  
   - **Training/Test Split**: 80% for training, 20% for testing.  

   **Dataset with New Class (HC Sand)**:  
   ![Multi-class Dataset](https://github.com/user-attachments/assets/69d58263-f8b7-4a60-aff4-e9fafac9bc8f)

2. **Model Training**  
   - A DNN model was trained for 20 epochs to learn the relationships among the three lithology classes.

3. **Results**  
   - The DNN successfully classified the test dataset into shale, sand, and HC sand:  
     ![Testing Results for Multi-class](https://github.com/user-attachments/assets/e22ae2ae-b9b1-4aa5-b46b-58b8319b47f4)

---

## Discussion

This project demonstrates the power of **Deep Neural Networks (DNNs)** to classify lithology using geophysical data, mimicking conventional rock physics workflows. Key takeaways include:

- **Learning without Physics**:  
  The DNN learned to separate lithologies based on the training data, without requiring explicit knowledge of rock physics principles like Ip vs. PR crossplots.
  
- **Confidence in Predictions**:  
  Prediction probabilities provided additional insights into model reliability and uncertainty.  

- **Scalability**:  
  The workflow can be extended to incorporate more classes, features, or datasets, showcasing the flexibility of DNNs in geoscience applications.

This approach demonstrates the potential for machine learning to enhance seismic interpretation, offering a robust alternative to traditional methods.

---
