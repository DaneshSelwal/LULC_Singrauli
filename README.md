# Land-Use Land-Cover Classification Singrauli 

This repository contains the code and data for land-use land-cover classification of the Singrauli district.

## ️ Google Earth Engine (GE)

This folder contains the JavaScript code exported from GEE. It exports the coordinates of the training dataset, the base image, and the Random Forest classified image.

[GEE](GEE)

##  Raw Data

This folder contains the raw data files directly exported from GEE.

[Link to Raw Data folder](Data/Raw_Data)

##  Tuned Data

This folder contains the train and test CSV files, which are the original raw data separated for use in the Classical ML script.

[Link to Tuned Data folder](Tuned_Data)

##  Classical Machine Learning (ML)

This folder contains the code for classical machine learning models. The first file performs hyperparameter tuning to find the best model. The second file contains the confusion matrices for all the models.

[Link to Classical ML folder](Classical_ML)

##  Convolutional Neural Network (CNN) Model

This folder contains the code for the CNN model. You can change the patch size from 10x10 to 64x64. The training notebook prepares the image patches and generates the confusion matrix. The prediction notebook generates the classified image.

[Link to CNN Model folder](CNN_Model)

##  Accuracy Assessment

This folder contains the script that takes thematic images from Random Forest and CNN models as input and generates a model accuracy report.

[Link to Accuracy Assessment folder](Accuracy_Assessment)
