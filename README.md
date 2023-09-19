# Detection-of-Covid-19-using-Speech-Analysis

## Overview
This project leverages deep learning techniques to classify COVID-19 positive and negative cases based on spectrogram images of voice samples. I utilized the convolutional neural Network and ResNet architecture, a well-known convolutional neural network (CNN), to perform this binary classification task. By fine-tuning a pre-trained model on our dataset, this project aims at providing an accurate and automated tool for COVID-19 diagnosis.

![Image of the project ](https://github.com/swati-sss/Detection-of-covid-19-using-speech/blob/main/covid-19%20project%20image.png?raw=true)

## Dataset
The dataset was downloaded from the "IISC Coswara Database" https://github.com/iiscleap/Coswara-Data. The Dataset consists of 9 type of voice samples of people who tested covid-positive and who tested covid negative. The voice samples consist sounds of "shallow breathing", "deep breathing", "light cough", "Heavy cough", "counting 1 to 10 fast", "counting 1 to 10 slow", "pronounciation of a", "pronounciation of o" and "pronounciation of e". This data is processed to generate MEL spectrograms of each voice sample and categorised as "positive" for COVID-19 positive cases and "negative" for COVID-19 negative cases. These images were obtained from voice samples, making it a non-invasive and accessible method for screening potential cases.

## Methodology
Data Preprocessing: We organize the dataset into training, validation, and test sets. Data augmentation techniques are applied to the training dataset to improve the model's generalization.

Transfer Learning: We employ a CNN model, which has demonstrated good performance on various image classification tasks. The model's convolutional layers are utilized as feature extractors, and we add custom fully connected layers to adapt it to our binary classification problem.

Model Training: The model is trained using the training dataset while monitoring its performance on the validation set. We employ binary cross-entropy loss and the Adam optimizer during training.

Evaluation: After training, the model's performance is evaluated on an independent test set using accuracy as the primary metric. Additional metrics such as precision, recall, and F1-score may also be used to assess its effectiveness.

## Usage
Clone this repository: git clone https://github.com/swati-sss/Detection-of-Covid-19-using-Speech-Analysis
Unzip the image dataset
Install the necessary dependencies.
Adjust hyperparameters and the number of training epochs in the code as needed.
Run the training script to fine-tune the CNN model on your dataset.
Evaluate the model's performance on the test set.

## Results
We present the results of our trained model, including accuracy and other relevant metrics, in the repository. Users can refer to these results to gauge the model's effectiveness. The accuracy achieved by CNN is 73%.

## Future Improvements
-Continuous monitoring and retraining with new data to maintain model accuracy.
-Deployment of the model as part of a diagnostic tool or healthcare system (Working on it).
-Integration of additional data sources and modalities for improved accuracy.

## Contributions
Contributions to this project are welcome. Feel free to submit issues, feature requests, or pull requests.
