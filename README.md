# rice-grain-classification-project
Classifying the two species of rice grain (Cammeo and Osmancik) using Logistic Regression.

User Manual
1. Development Environment
This project can be run using Google Colab or Jupyter Notebook. Python 3 is required to execute the notebook and train the Logistic Regression model. Google Colab is recommended because it provides an online Python environment and does not require a local Python installation.

The project uses the following Python libraries:

liac-arff
pandas
matplotlib
seaborn
scikit-learn
If the required libraries are not installed, they can be installed using:

pip install liac-arff pandas matplotlib seaborn scikit-learn

2. Required Files
The following files are required:

rice-grain-classification.ipynb
Rice_Cammeo_Osmancik.arff
The notebook file contains the Python source code, while the ARFF file contains the rice grain dataset used for training and testing.

The dataset file name must match the file name used in the notebook code:

Rice_Cammeo_Osmancik.arff

3. Running the Project
Open Google Colab or Jupyter Notebook.
Open rice-grain-classification.ipynb.
If Google Colab is used, upload Rice_Cammeo_Osmancik.arff to the Colab working directory.
Run the package installation cell if required.
Run all notebook cells from top to bottom in order.
Do not skip the data preprocessing, train-test split, or feature scaling cells.
Wait for each cell to finish before continuing to the next cell.
In Google Colab, the user can also select:

Runtime → Run all

after the dataset has been uploaded.

4. Model Training and Testing
The notebook first loads and explores the rice grain dataset.

The class labels are converted into numerical values:

Osmancik = 0
Cammeo = 1
The dataset is then divided into training and testing sets. 80% of the data is used for training and 20% is used for testing.

The numerical features are standardised using StandardScaler.

A Logistic Regression model is then trained using the training dataset and tested using the testing dataset.

5. Expected Results
After the notebook is executed successfully, the user should be able to see:

Dataset information
Data distribution graphs
Training and testing accuracy
Precision
Recall
F1-score
Classification Report
Confusion Matrix
Confusion Matrix visualisation
ROC Curve
The current model achieves approximately:

Training Accuracy: 93.21%
Testing Accuracy: 92.13%
These results show the performance of the Logistic Regression model in classifying Cammeo and Osmancik rice grains.

6. Troubleshooting
If a FileNotFoundError occurs, check that Rice_Cammeo_Osmancik.arff has been uploaded and that the file name matches the notebook code exactly.

If the arff library cannot be imported, install it using:

pip install liac-arff

If variables such as X_train, y_test, or lr are not defined, some earlier cells may have been skipped. Run the notebook again from the top.

If Google Colab is restarted or disconnected, the ARFF dataset may need to be uploaded again.
