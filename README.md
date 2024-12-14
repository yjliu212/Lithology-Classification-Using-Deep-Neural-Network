# Lithology-Classification-Using-Deep-Neural-Network

## [Notebook 1](https://github.com/yjliu212/Lithology-Classification-Using-Deep-Neural-Network/blob/main/Assignment_3_Lithology_Classification_Prediction.ipynb)

In this experiment, we carried out lithology classification based on Vp, Density and Poisson Ratio (PR) training data with classified data points, where 0 represents shale, and 1 represents sand in the first Notebook.

The dataset was created by randomly sample Vp, Density and PR within a certain range. As shown below:
![image](https://github.com/user-attachments/assets/f2cedcbc-f850-407c-8f1a-44ff6e770fb2)
![image](https://github.com/user-attachments/assets/2900ecbb-188d-43ef-93f8-c8971a17d62a)
![image](https://github.com/user-attachments/assets/f58b539e-f0f3-4e88-8942-f7312e794f97)

Then, the training data classification was created by seperating sand from shale based on a rock physics model. This created our training dataset. The training dataset was partitioned into 80% for training and 20% for testing.
![image](https://github.com/user-attachments/assets/60928499-5656-4b68-8af7-ef1d397b5fec)

**Deep Neural Network (DNN)**

**Result**

After 10 epochs, the DNN model captured the partern and successfully seperated the data points in the testing dataset:
![image](https://github.com/user-attachments/assets/4c3a348d-f1c0-4144-94b1-7a115d4ca59c)

The prediction confidence are also generated:
![image](https://github.com/user-attachments/assets/af4b25a8-c109-4759-9689-698b7589a395)


