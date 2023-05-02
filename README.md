# NASA Engine Failure Prediction

This project uses machine learning techniques to predict when an aircraft engine is likely to fail, based on sensor readings from the engine. The data used in this project is provided by NASA, and contains measurements from a fleet of engines which were run to failure in a controlled environment. 

## Data Description

The dataset contains sensor readings from 100 aircraft engines, with each engine having a different number of cycles until failure. The data is split into two sets: a training set with 20,631 rows and a test set with 13,000 rows. The training set is used to train the machine learning model, and the test set is used to evaluate the model's performance. There is also a separate file with the remaining useful life (RUL) of each engine in the test set.

## Methods Used

The project uses a random forest regression model to predict the RUL of each engine in the test set. Before training the model, the data is preprocessed to remove any NaN values and scale the sensor readings using a standard scaler. The model is then trained on the preprocessed data, and its performance is evaluated using mean squared error (MSE) and R-squared (R2) metrics.

## Results

The final model achieves an MSE of 26.59 and an R2 score of 0.59 on the test set, indicating good performance in predicting the remaining useful life of each engine. The project also includes visualizations of the data to better understand the distribution of sensor readings and the relationship between engine cycles and failure.

## How to Use

To use this project, simply clone the repository and run the `nasa-predictive-maintenance-rul.ipynb` Jupyter notebook. The notebook contains all the code used in the project, as well as detailed explanations of each step.

## Dependencies

The project requires the following libraries to be installed:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- random
- warnings

These libraries can be installed using pip.


## Credits

This project was created by Naman Mistry. The dataset used in this project was provided by NASA through the Prognostics Data Repository. 

