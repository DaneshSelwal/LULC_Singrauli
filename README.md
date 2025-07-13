# Land-Use Land-Cover Classification Singrauli 

This repository contains the code and data for land-use land-cover classification of the Singrauli district.

## ️ Google Earth Engine (GEE)

This folder contains the [JavaScript code](GEE/GEE_Script.js) exported from GEE. It exports the coordinates of the training dataset, the base image, and the [Random Forest classified image](GEE/Singrauli_LULC_Classified_RF_2024.tif).

##  Raw Data

This folder contains the raw data files directly exported from GEE.

[Raw Data](Raw_Data)

##  Tuned Data

This folder contains the train and test CSV files, which are the original raw data separated for use in the Classical ML script.

[Tuned Data](Tuned_Data)

##  Classical Machine Learning (ML)

This folder contains the code for classical machine learning models. The [classical ML](Classical_ML/Optuna_autosampler_Singrauli.ipynb) file performs hyperparameter tuning to find the best model. The [results](Classical_ML/test_results.xlsx) file contains the confusion matrices for all the models.

##  Convolutional Neural Network (CNN) Model

This folder contains the code for the CNN model. You can change the patch size from 10x10 to 64x64. The [training notebook](CNN_Model/CNN_Training/cnn-training.ipynb) prepares the image patches and generates the confusion matrix. The [prediction notebook](CNN_Model/CNN_Prediction/cnn-prediction.ipynb) generates the classified image.

##  Accuracy Assessment

This folder contains the [script](Accuracy Assessment/Accuracy_assessment.ipynb) that takes [thematic images](Accuracy Assessment/Thematic_images) from Random Forest and CNN models as input and generates a model [accuracy report](Accuracy Assessment/model_accuracy_report.docx).

