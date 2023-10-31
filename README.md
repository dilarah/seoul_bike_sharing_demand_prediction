# Seoul bike sharing demand prediction

About the Dataset:

This project is about the predicted number of bikes rented at a specific hour of the day/year. <br>
Source: https://www.kaggle.com/datasets/saurabhshahane/seoul-bike-sharing-demand-prediction/data <br>
A quick summary of the dataset can be found below: <br>

1. There are 14 features with 8760 rows of data. <br>
2. There are 4 categorical columns and 10 numerical columns. Columns ‘Date’, ‘Seasons’, and ‘Functioning Day’ are of 𝑜𝑏𝑗𝑒𝑐𝑡 data type. <br>
3. Columns ‘Rented Bike Count’, ‘Hour’, ‘Humidity (%)', and ‘Visibility (10𝑚)' are of 𝑖𝑛𝑡64 numerical data type. <br>
4. Columns ‘Temperature Temperature (℃)’, ‘Wind Speed (𝑚/𝑠)’, ‘Dew Point Temperature (℃)’, ‘Solar Radiation (𝑀𝐽/𝑚2)’, ‘Rainfall (𝑚𝑚)' and ‘Snowfall(𝑐𝑚) are of 𝑓𝑙𝑜𝑎𝑡64 numarical data type. <br>

## Data Analysis

- No missing data are found in the dataset.
  
- No duplicates are found in the dataset.
  
- Categorical Data:
  
Unique count: Seasons- 4, Holiday- 2, Functioning Day- 2, will later be one hot encoded with dropping when binary 

- Numerical Data:

Distribution of most of the data is not normally distributed and includes a lot of outliers. Later will be Robust scaled to eliminate the outlier effect.

- Correlation Matrix
![corr matrix](https://github.com/dilarah/seoul_bike_sharing_demand_prediction/assets/33967361/b1783674-d9af-4f7e-953d-9b38bf8d6021)

When the all Pearson correlation is listed to predict the target some features appear to have higher correlation.

    Temperature(C)              0.538558
    Seasons_Winter              0.424925
    Hour                        0.410257
    Dew point temperature(C)    0.379788
    Seasons_Summer              0.296549
    Solar Radiation (MJ/m2)     0.261837

## Data Visualisation

Hourly distribution of average rented bike count

![download (1)](https://github.com/dilarah/seoul_bike_sharing_demand_prediction/assets/33967361/ec9a7f85-97f1-4dee-a145-b2f73d111b0c)

Daily distribution of average rented bike count (From Monday to Sunday)

![2](https://github.com/dilarah/seoul_bike_sharing_demand_prediction/assets/33967361/5f3f2f56-49c3-4bab-ac4f-ffdca518b4ab)

Monthly distribution of average rented bike count 

![download (2)](https://github.com/dilarah/seoul_bike_sharing_demand_prediction/assets/33967361/ec3d8184-6436-43c0-ae2f-beb6a2f65cdc)

Seasonal distribution of average rented bike count 

![download (4)](https://github.com/dilarah/seoul_bike_sharing_demand_prediction/assets/33967361/e427014c-288e-41bf-a6bc-2f9e14bd850e)

Holiday/Not Holiday rented bike distribution

![download (5)](https://github.com/dilarah/seoul_bike_sharing_demand_prediction/assets/33967361/1a347144-90c5-4247-b04b-2191b85499b4)


