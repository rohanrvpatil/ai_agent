## AI agent for sentiment analysis on Rotten Tomatoes dataset:

### 1. Introduction
The sentiment analysis project aims to develop a machine learning model capable of classifying the sentiment (positive or negative) of text data, particularly movie reviews. The project utilizes deep learning techniques, specifically Long Short-Term Memory (LSTM) networks, to perform sentiment analysis on textual input.

### 2. Problem Statement
The project addresses the challenge of sentiment classification in movie reviews. By accurately classifying the sentiment conveyed in text data, the model can assist in analyzing audience reactions, identifying trends, and providing insights into the overall sentiment towards movies.

### 3. Data Collection and Preprocessing
Data is collected from the Rotten Tomatoes Movie Reviews dataset, which contains a collection of movie reviews along with their sentiment labels.
The dataset is preprocessed to remove noise, tokenize the text, and pad sequences to ensure uniform length.

### 4. Model Development
The sentiment analysis model is developed using TensorFlow's Keras API.
The model architecture consists of an embedding layer, followed by a SpatialDropout1D layer, an LSTM layer, and a Dense layer with a sigmoid activation function.
Hyperparameters such as the number of LSTM units, dropout rates, and optimizer are tuned to optimize model performance.

### 5. Training
The dataset is split into training and testing sets using a train-test split ratio of 80:20.
The model is trained on the training set and validated on the testing set for a total of 30 epochs.
Training progress and performance metrics such as loss and accuracy are monitored during training.

### 6. Evaluation
The trained model is evaluated on the testing set to assess its performance.
Performance metrics such as accuracy are computed to measure the model's effectiveness in sentiment classification.

### 7. Deployment
Once trained and evaluated, the sentiment analysis model is saved to disk in the HDF5 format (sentiment_model.h5).
The saved model can be loaded and used for making real-time predictions on new text data, as demonstrated in the provided code snippet.

### 8. Conclusion
The sentiment analysis project successfully develops a deep learning model for sentiment classification in movie reviews. By leveraging LSTM networks and the Rotten Tomatoes Movie Reviews dataset, the model demonstrates strong performance in accurately classifying sentiment. Future work may involve fine-tuning the model, exploring additional datasets, and deploying the model in real-world applications.
