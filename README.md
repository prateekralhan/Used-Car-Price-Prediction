# Used Car Price Prediction 🏎🚙⛽️ [![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![](https://img.shields.io/badge/Prateek-Ralhan-brightgreen.svg?colorB=ff0000)](https://prateekralhan.github.io/)

A ML based Web application that helps in predicting the *selling price* of a used 🚗 🚙

## Live Web-App available [here.](https://car-price-predict-app.herokuapp.com/)

### Dataset
You can find the dataset [here.](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho)

### Installation:
Simply execute the command: ***pip install -r requirements.txt*** to install the necessary dependencies.

### Usage:
1. Clone this Repository to a directory and navigate to that directory.
2. Run the command: ***python app.py***
3. This will run the web-app on localhost and would look something like this. Feel free to play around with the codes, add more features, beautify it. :wink:

<kbd>
<img src="https://user-images.githubusercontent.com/29462447/103283342-54504680-49fe-11eb-9a03-5695d925600b.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/103283342-54504680-49fe-11eb-9a03-5695d925600b.png"/> 
</kbd>

&nbsp;
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/103283363-616d3580-49fe-11eb-9343-7a72872e1048.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/103283363-616d3580-49fe-11eb-9343-7a72872e1048.png"/> 
</kbd>

### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build --tag car_price_prediction_app .
```
4. Run the docker:
```
docker run --publish 8000:8080 --detach --name bb2 car_price_prediction_app
```

This will launch the dockerized app. Navigate to ***localhost:8000*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
