# Synthetic_Series_Data
This notebook presents a series of functions for generating synthetic time series data. We attempt to simulate time series as realistic as possible with different shapes, frequency, period and with characterisitcs as non-stationarity, seasonality, trend and different kinds of anomalies.


Variables used as args¶<br />
timestamps = timestamps for the seasonality pattern<br />
thres = timestamps that are the thresholds for the appearance of the first triangle<br />
exp1 = exponent of the time for the generation of the first triangle<br />
subtr1 = subtrahend to subtract from the time<br />
exp2 = the exponent for the previous operation to create the second traingle<br />
timesteps_all = the overall timesteps of the time series. It should have a perfect division with timestamps variable.<br />
number_outl = number of outliers that we want to generate<br />
thres1 = the lowest threshold for the generation of outlier. Specifically the the lowest number that will multiply the standard deviation. Based on the theory must be > |3|<br />
thres2 = the highest threshold for the multiplier of the standard deviation. It must be >= thres1.<br />
y = a multiplier for creating the trend<br />
z = a multiplier for generating the noise<br />
chunksize = the length of the plateau in timestamps<br />
number_plat = number of plateaus<br />
lim1= the starting timestamp for the contextual anomalies<br />
lim2=the ending timestamp for the contextual anomalies<br />
gen_out = boolean variable for generating outliers<br />
plateau = boolean variable for generating plateaus<br />
context = boolean variable for generating contextual anomalies<br />
