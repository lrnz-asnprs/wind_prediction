# Wind Prediction Project

Within this project I have implemented a data preprocessing pipeline for a small wind energy forecasting system using sklearn. I'd used data from Orkney, an archipelago off the north eastern coast of Scotland. Orkney has around 20,000 inhabitants and they produce around » 120% of their annual energy consumption in wind energy.

## Usage

Simply go ahead and run the cells in the notebook to generate the predictions and plots.
The project includes data exploration and visualization, a data preprocessing pipeline using sklearn and an comparison of the accuracy of a polynomial regression model versus K-nearest neighbors using KFold cross validation.

## Results

Since the correlation between wind speed and total energy produced is not clearly linear, I used a polynomial transformation to better fit the models (Linear Regression and K-Nearest Neighbors) to the underlying data. As a result I was able to fit my model to a polynomial line as depicted in the figure below. 

![alt text](https://github.com/lrnz-asnprs/wind_prediction/blob/master/output_ln.png?raw=true)

I used k-fold cross validation to compare the performance of the two models I have implemented. It turns out that KNN performs slightly better (ME=0.653, SE=0.023) than the Linear Regression (ME=0.652, SE=0.020). However, accuracy is rather low for both models, due to the high variance of the data and the simplicity of the models.

### Dependencies
Libraries used:
* Pandas & NumPy
* Sklearn
* Matplotlib & Seaborn
