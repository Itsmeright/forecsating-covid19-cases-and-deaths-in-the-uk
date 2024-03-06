# Forecsating-covid19-cases-in-the-uk
<h1>Description</h1>
<p>The aim of the project is to forecast future covid-19 cases and deaths in the united kingdom usin various machine learning and deep learning models. 
  The project compares the accuracy of different models that has been used for forecasting. The forecast is for the entire as well as the four regions that make the uk namely:
England, Scotland, Northern Ireland and Wales.</p>
<h1>Dataset</h1>
<p>The dataset used for this project is the data collected by Oxford COVID-19 Government Response Tracker, Blavatnik School of Government, University of Oxford. The data collected contains data for 185 different countries. However, the data for the united kingdom as a whole and the four regions of the united kingdom is 5480 rows spanning from 2020 to 2022
</p>
<h2>Data preprocessing</h2>
<p>
  To prepare the data for modelling i had to do some cleaning by changing datatype to the appropriate datatype. I also dealt with missing values by filling the missing value with the average of the previous and the next value. I splitted the dataset into each of the juridistion in the dataset namely; national, England, Scotland, Wales and Northern Ireland so as to predict each of thes jurisdiction appropriately.
</p>
<h2>Modelling and Evaluation</h2>
<p>
  The models used for this project include Arima, facebook prophet, LSTM, CNN-LSTM. Modelling was done in a rolling forecast to shift the window and predict only the next day and then the window of the training data shifts. In order to make the data stationary for the ARIMA model, i used first order differencing and then AIC was used to choose the best order for the ARIMA model.  
   
</p>

<p>
  In order to use the facebook prophet model, the column names have to be changed to ds for the date column and s for the value to be predicted. LSTM AND CNN-LSTM were implemented from the tensorflow library.
  ARIMA model performed best for most of the regions and LSTM also performed better than cnn-lstm.
</p>
