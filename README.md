# Neural_Network_Charity_Analysis
# Overview 
The purpose of the analysis was to train a neural network for the Alphabet Soup charity analysis. 
#Results
## Data Preprocessing  
First the charity_data.csv file was loaded into a Pandas DataFrame and performed data preprocessing tasks, including dropping the non-beneficial ID columns, converting categorical variables to numeric using one-hot encoding, and scaling the data.

## Compiling, Training, and Evaluating the Model 
Then the data was compiled and trained a deep learning neural network model using TensorFlow Keras. The model consisted of two hidden layers, each with 80 neurons and the rectified linear unit (ReLU) activation function, and an output layer with one neuron and the sigmoid activation function. The model was trained for 100 epochs using the binary cross-entropy loss function and the Adam optimization algorithm. Finally, the model was evaluated using the test data and calculated the loss function value and accuracy score.

![Visualize the value counts of CLASSIFICATION](https://github.com/aahudson/Neural_Network_Charity_Analysis/blob/main/Resources/Classification_Counts_Density.png)
- [First Attempt to Train Model](https://github.com/aahudson/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb)
- [Optimized Model](https://github.com/aahudson/Neural_Network_Charity_Analysis/blob/main/OptimizedAlphabetSoupCharity.ipynb)
# Summary 
## The accuracy test showed the following results for the first attempt: 
268/268 - 1s - loss: 0.5648 - accuracy: 0.7285 - 637ms/epoch - 2ms/step
Loss: 0.5648044943809509, Accuracy: 0.7285131216049194
This means that about 72.85% of the predictions made by the model were correct. The loss function value is 0.5648, which indicates how well the model is able to minimize the difference between the predicted and actual target values. A lower loss function value indicates a better model performance.
## The accuracy test showed the following results for the optimized model attempt: 
mean 268/268 - 1s - loss: 0.5604 - accuracy: 0.7282 - 595ms/epoch - 2ms/step
Loss: 0.5604255199432373, Accuracy: 0.7281632423400879
The new accuracy rate after optimizing the model is 72.82%, which is slightly lower than the original accuracy rate of 72.85%. This means that the optimization techniques used did not significantly improve the model's performance. However, it is still possible that the model is now more efficient or stable with the changes that were made.
