# Synthetic_Series_Data
This notebook presents a series of functions for generating synthetic time series data. We attempt to simulate time series as realistic as possible with different shapes, frequency, period and with characterisitcs as non-stationarity, seasonality, trend and different kinds of anomalies.


Variables used as args¶
timestamps = timestamps for the seasonality pattern
thres = timestamps that are the thresholds for the appearance of the first triangle
exp1 = exponent of the time for the generation of the first triangle
subtr1 = subtrahend to subtract from the time
exp2 = the exponent for the previous operation to create the second traingle
timesteps_all = the overall timesteps of the time series. It should have a perfect division with timestamps variable.
number_outl = number of outliers that we want to generate
thres1 = the lowest threshold for the generation of outlier. Specifically the the lowest number that will multiply the standard deviation. Based on the theory must be > |3|
thres2 = the highest threshold for the multiplier of the standard deviation. It must be >= thres1.
y = a multiplier for creating the trend
z = a multiplier for generating the noise
chunksize = the length of the plateau in timestamps
number_plat = number of plateaus
lim1= the starting timestamp for the contextual anomalies
lim2=the ending timestamp for the contextual anomalies
gen_out = boolean variable for generating outliers
plateau = boolean variable for generating plateaus
context = boolean variable for generating contextual anomalies
