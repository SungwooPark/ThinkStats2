# Is There a Seasonality in Number of Likes for Social Media Posts?

Using a dataset containing over 4 million facebook posts from 15 mainstream news outlets, I investigate the existence of seasonality in the number of likes a facebook post from a news outlet gets. The dataset contains contents and attributes, such as number of likes and timestamp, of all facebook posts posted by the media sources from 2012 to 2016. The media outlets included in the data are ABC, BBC, CBS, CNN, Fox & Friends, Fox, LA Times, NBC, NPR, The Huffington Post, The New York Times, The Wall Street Journal, The Washington Post, Time, and USA Today.

## Methodology

I extract the number of likes and timestamp from all posts in the dataset. The dataset is structured into several separate collections of posts from different media outlets, so I end up with collections of number of likes and timestamps, in which each collection represents a different media outlet. I then convert each timestamp into a numerical 'year' value, which is a number of years since the time first post from the corresponding media outlet was posted. In order to accurately investigate the existence of seasonality, I subtract the trend from my data. To do this, I compute the residuals by subtracting exponentially weighted moving average from the time series of number of likes. Lastly, I compute autocorrelation function for the residuals and investigate the serial correlation values for lag of 1, 7, 30, and 365 days.

## Results and Intepretation

Following is a table summarizing the serial correlation values of the number of likes from different media outlets.

| Media Outlet | 1 Day | 7 Days | 30 Days | 365 Days |
| --- | --- | --- | --- | --- |
| CNN | -0.029756534977066724 | -0.0004785693401439372 | -0.0006886404933035297 | -0.002546237951539804 |