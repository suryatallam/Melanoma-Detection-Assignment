# Project Name
> Outline a brief description of your project.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths
- A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Analysis from the Conclusion 1 :
Accuracy:
The training and validation accuracy curves both increase over the epochs, reaching around 59.05% for training and 54.59% for validation at the last epoch. This indicates that the model is   learning, but the accuracy levels suggest that there may be room for improvement, possibly due to model capacity, data quality, or other factors. The gap between training and validation accuracy is relatively small, indicating that overfitting might not be a significant issue.

Loss:
The training and validation loss both decrease over time, but the validation loss fluctuates more and is consistently higher than the training loss towards the end. This slight increase in the validation loss curve while the training loss continues to decrease can sometimes indicate early signs of overfitting. The difference between training and validation loss by the end suggests that the model might be fitting slightly better on the training data, which is typical but something to watch for with more training epochs.

Overfitting/Underfitting:
Given the small difference between training and validation metrics, there's no strong evidence of overfitting. However, the model might not have learned enough to generalize well, which can be a form of UNDERFITTING. The model’s relatively low accuracy suggests that it could benefit from further tuning, potentially by increasing its complexity, improving data preprocessing, or experimenting with other architectures.

- Analysis from the Conclusion 2 :
  Even though Agumented the data with ImageDataGenerator still  the Model is UNDERFITTING because having Train Accuracy 51.02% and Validation Accuracy 47.74%.At its current state, the model is not performing well. Focus on improving the data, model architecture, or training process to boost performance.
   Steps to Improve:
1. Examine Data:
Class Imbalance: Ensure that the dataset is balanced or use techniques like oversampling/undersampling or class-weight adjustments.
2. Adjust Model Complexity:
Increase Complexity: If the model is underfitting, try a more complex model (e.g., deeper neural networks, ensemble methods like Random Forests, or XGBoost).
3. Improve Training Process:
Longer Training: Train the model for more epochs, but monitor for overfitting.

- Analysis from the Conclusion 3 :
  After Handling the Class imbalance by adding the Agumented data, Model was get rid of UNDERFITTING.
  Train Accuracy: 0.9127 (91.27%):
1. The model performs well on the training data, capturing the majority of patterns.
2. Train Loss: 0.2576:A relatively low loss value indicates that the model predictions align closely with the actual labels in the training set

Validation Accuracy: 0.9545 (95.45%):
A higher validation accuracy than training accuracy suggests the model generalizes well to unseen data. This is usually a good sign.
Validation Loss: 0.1422:
1. The validation loss is significantly lower than the training loss, which can indicate:
2. The model may generalize better to the validation data.
3. The validation set might be simpler or less noisy compared to the training data.
Performance Perspective:
1. The accuracy values are high for both training and validation, suggesting that the model is likely effective for its intended purpose.
2. The lower validation loss compared to training loss further supports that the model generalizes well to unseen data.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- library - Pandas version: 2.2.2
- library - NumPy version: 1.26.0
- library - Matplotlib version: 3.9.2
- library - OS module version: Not applicable (built-in module)
- library - Pillow (PIL) version: 10.4.0
- library - Augmentor version: 0.2.12

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
The UpGrad course materials on Convolutional Neural Networks were used as reference while designing and analyzing the problem statement.

## Contact
Created by Surya [https://github.com/suryatallam] - feel free to contact us!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
