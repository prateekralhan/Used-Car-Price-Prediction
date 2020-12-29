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
<p>
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/103284748-19e8a880-4a02-11eb-9f6c-cef42524645e.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/103284748-19e8a880-4a02-11eb-9f6c-cef42524645e.png"/> 
</kbd>  

<kbd>
<img src="https://user-images.githubusercontent.com/29462447/103284753-1d7c2f80-4a02-11eb-880e-49e456f1c497.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/103284753-1d7c2f80-4a02-11eb-880e-49e456f1c497.png"/> 
</kbd>  
</p>
<p align="center">
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/103285194-713b4880-4a03-11eb-9cfa-78115cc8b27b.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/103285194-713b4880-4a03-11eb-9cfa-78115cc8b27b.png"/> 
</kbd>
</p>
<hr>
<strong> Metrics ( Final Model )</strong>
<br>
<table>
  <tr>
    <th>Metric</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>MAE</td>
    <td>1.0406</td>
  </tr>
  <tr>
    <td>MSE</td>
    <td>5.7957</td>
  </tr>
    <tr>
    <td>RMSE</td>
    <td>2.4074</td>
  </tr>
  <tr>
    <td>R2</td>
    <td>0.8413</td>
  </tr>
</table>

1. MAE  : 1.0406058674433205
2. MSE  : 5.795724771873122
3. RMSE : 2.4074311562063664
4. R2   : 0.8413277571195945
<hr>
