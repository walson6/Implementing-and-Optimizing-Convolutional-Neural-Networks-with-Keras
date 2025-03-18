###  Project Title: Implementing and Optimizing Convolutional Neural Networks with Keras

**Objective:** 
To practice using the Keras package for implementing and optimizing Convolutional Neural Networks (CNNs) on the CIFAR-10 dataset.

**Implementation:**
1. **Data Preparation:**
   - Loaded the CIFAR-10 dataset from Keras.
   - The dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class.
   - Split the data into training (50,000 images) and test (10,000 images) sets.
   - Preprocessed the data by scaling pixel values to the range [0, 1] and converting labels to one-hot encoding.
2. **Model Training and Evaluation:**
   - Simple CNN Model (cnn1):
       - Architecture: Two convolutional layers with max-pooling, followed by a flatten layer and a dense output layer.
       - Trained for 50 epochs with a batch size of 128.
       - Achieved a test accuracy of 68.94%.
   - CNN with Dense Hidden Layer (cnn2):
       - Added a dense hidden layer with 128 neurons and ReLU activation before the output layer.
       - Trained for 50 epochs with a batch size of 128.
       - Achieved a test accuracy of 66.11%.
       - Observation: The model overfitted, as indicated by the high training accuracy and lower validation accuracy.
   - CNN with Dropout (cnn3):
       - Added dropout layers with a dropout rate of 0.25 after the flatten layer and the dense hidden layer.
       - Trained for 50 epochs with a batch size of 128.
       - Achieved a test accuracy of 73.51%.
       - Observation: Dropout helped reduce overfitting and improved generalization to new data.
   - Optimized CNN (cnn4):
       - Increased the number of convolutional layers and adjusted the number of filters.
       - Added dropout layers with varying dropout rates.
       - Trained for 50 epochs with a batch size of 128.
       - Achieved a test accuracy of 75.78%.
       - Observation: The model showed improved performance with more convolutional layers and optimized dropout rates.

3. **Model Evaluation:**
   - Evaluated each model on the test set to measure accuracy and loss.
   - Used confusion matrices and visualizations to analyze model performance.

**Skills Demonstrated:**
- Proficiency in Python and Keras.
- Understanding of Convolutional Neural Networks and their architecture.
- Experience with data preprocessing and scaling.
- Knowledge of regularization techniques (dropout) to prevent overfitting.
- Ability to optimize model performance through hyperparameter tuning.

**Tools and Libraries Used:**
- Python
- Keras
- NumPy
- Matplotlib
- Scikit-learn
