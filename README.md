# Handsign Recognition 🤚
<div align="center">
  <img src="https://github.com/dinata16/data-science-projects/assets/89764786/17476a6a-54d2-431e-9021-6305176495ab" alt="creditcard">
</div>

## Project Overview 📑
Many people do not understand the use of sign language, so when interacting with someone who is speech impaired, difficulties in communication will arise. Sign language is the primary means of communication for the hearing impaired. However, the general public's recognition of sign language is still limited. Therefore, This project aims to develop a machine learning model capable of detecting American Sign Language Handsign and classifying them into corresponding letters. The purpose of this project is to help people learn and understand handsign easily, serving as a baseline model for future improvements. 


## About The Dataset ✏
The project utilizes [ASL Dataset](https://www.kaggle.com/datasets/ayuraj/asl-dataset/data) from Kaggle which contains images of hand signs for both numbers and letters from A-Z. However, since the model is focused on classifying letters, the numbers are discarded from the dataset.

## Methodology 🍴
- Data Preprocessing: Pipelining image into a dataset, splitting dataset to train, test, and validation, and address image preprocessing (e.g., shuffling, scaling, and batching images).
- Modeling: Develop machine learning model using transfer learning from VGG16 and conduct experiments to find the most suitable combination of layer for building a robust model
- Fine Tuning: Experimenting to find the optimal hyperparameters to help model converge faster
- Model Evaluation: Evaluate model performance using metrics like precision, recall, F1-score, Accuracy and confusion matrix 

## Results ⭐
The loss and accuracy metrics from the training and validation data show excellent results, indicating that the model is improving with each epoch. This consistent learning demonstrates the effectiveness of the training process and suggests that the model is successfully capturing the underlying patterns in the data. 
![Training and Validation of model](/assets/images/electrocat.png)

then using confusion matrix it is shown that the model is able to predict each class from test set accurately with only 1 missclassification.
![Confusion Matrix](/assets/images/electrocat.png)

I then test the model using random handsign images from the internet to see how accurate would the model be in classifying random images:
1. ![L](/assets/images/electrocat.png)
2. ![G](/assets/images/electrocat.png)
3. ![C](/assets/images/electrocat.png)

## Conclusion 💾
This project demonstrates the potential of machine learning in hand sign detection. The developed model can be a valuable tool to assist deaf people in communicating, learning, and performing various tasks more effectively.

## Suggestions 📎
- Experiment with more complex model architectures and other transfer learning models.
- Collect more data to improve model performance.
- Develop a real-time system to detect handsign using camera with bounding boxes.
- Develop a more complex logic to stitch together the letters to make a word.

## Contributions 👨‍🔧
Contributions are welcome! Please submit a pull request if you have any suggestions or improvements.
