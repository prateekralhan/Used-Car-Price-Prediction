# Used Car Price Prediction

Live Web-App available [here.](https://car-price-predict-app.herokuapp.com/)

## Dataset
You can find the dataset [here.](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho)

## Installation:
Simply execute the command: ***pip install -r requirements.txt*** to install the necessary dependencies.

## Usage:
1. Clone this Repository to a directory and navigate to that directory.
2. Run the command: ***jupyter notebook*** in the command prompt/terminal/powershell.
3. Feel free to explore the EDA and Modelling done by me as well as make further changes/refinements as per your innovative ideas :smile:

### Model:
* I implemented 3 Models initially which yielded the following results:

| **Model Name**  | **Linear Regression** | **Decision Tree Regression** | **Random Forest Regression** |
| --------------- | --------------------- | ---------------------------- | ---------------------------- |
| MAE             | 1.2093                | 0.5868                       | **0.4063**                   |
| MSE             | 2.6698                | 1.4126                       | **0.4376**                   | 
| RMSE            | 1.6339                | 1.1885                       | **0.6615**                   |
| R2              | 0.8516                | 0.9214                       | **0.9756**                   |
  
Thus, we plan to go forward with the Random Forest Regression Algorithm further :wink:

### Multi-Core Model Training and HyperParameter Tuning
The Model was trained progressively with increasing number of Physical/Logical Cores *(Intel i7 7th Gen 700 CPU 12 GB DDR4 RAM)* as well as further subjected to multi-core hyperparameter tuning for getting best possible values for the model using **RandomizedSearchCV** methodology.

