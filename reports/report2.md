# Is There a Seasonality in Number of Likes for Social Media Posts?

Using a dataset containing over 4 million facebook posts from 15 mainstream news outlets, I investigate the existence of seasonality in the number of likes a facebook post from a news outlet gets. The dataset contains contents and attributes, such as number of likes and timestamp, of all facebook posts posted by the media sources from 2012 to 2016. The media outlets included in the data are ABC, BBC, CBS, CNN, Fox & Friends, Fox, LA Times, NBC, NPR, The Huffington Post, The New York Times, The Wall Street Journal, The Washington Post, Time, and USA Today.

## Methodology

I extract the number of likes and timestamp from all posts in the dataset. The dataset is structured into several separate collections of posts from different media outlets, so I end up with collections of number of likes and timestamps, in which each collection represents a different media outlet. I then convert each timestamp into a numerical 'year' value, which is a number of years since the time first post from the corresponding media outlet was posted. In order to accurately investigate the existence of seasonality, I subtract the trend from my data. To do this, I compute the residuals by subtracting exponentially weighted moving average from the time series of number of likes. Lastly, I compute autocorrelation function for the residuals and investigate the serial correlation values for lag of 1, 7, 30, and 365 days.

## Results and Intepretation

Following is a table summarizing the serial correlation values of the number of likes from different media outlets.

| Media Outlet | 1 Day | 7 Days | 30 Days | 365 Days |
| --- | --- | --- | --- | --- |
| CNN | -0.029756534977066724 | -0.0004785693401439372 | -0.0006886404933035297 | -0.002546237951539804 |
| The Huff Post | 0.014442282792503917 | -0.026183919462200732 | -0.007970192420518305 | -0.00019594467253888708 |
| LA Times | -0.031138879018477013 | -0.008998078485048548 | -0.0042169043615362225 | -0.003682419291510698 |
| NPR | -0.027428518881018975 | -0.025808008785235252 | -0.006584060781139451 | -0.006376719346369967 |
| NBC | -0.019437874239638102 | -0.028276027511564595 | -0.006532568617991822 | 0.005096078582649778 |
| Fox | -0.004308856610576095 | -0.008457467641435866 | -0.0007433323062722195 | -0.012392345085506525 |
| Fox and Friends | -0.004017589133827942 | -0.0315307119193414 | -0.002057091266958815 | 0.0059177877708477 |
| CBS | -0.03166688187731559 | -0.021754249811873547 | -0.0024094556462089895 | 0.0010374684103873722 |
| BBC | -0.03044649917022163 | -0.011723564005179135 | 0.001962994900976816 | -0.010021557847552898 |
| ABC | -0.014955579272878328 | -0.02757913719934127 | -0.013540009034600455 | -0.0041998277455368715 |
| WSJ | -0.027456333237942856 | -0.01646119476436739 | -0.006950547709207333 | -0.002729155993090073 |
| NYT | -0.014782481757562253 | -0.0008041267638878915 | -0.0023373725413949925 | 0.006418153244978329 |
| The Washington Post | -0.020166667924224203 | -0.027377831942780817 | -0.014020351104383995 | -0.001392318016343383 |
| Time | -0.021322859342308716 | -0.01729191409269437 | -0.008359143931852168 | -0.0040691125244319195 |
| USA Today | -0.024658035151354982 | -0.019656236403451436 | -0.016058607242599932 | -0.0068374022853718635 |

All serial correlation values are small, indicating that there are no significant daily, weekly, monthly, or yearly serial correlation. 

## Conclusion
When I compute the serial correlation values for the time series of number of likes for media outlet social media posts, the computed values are very small. Small serial correlation values suggests that there is no serial correlation of any sort among number of likes that a media outlet's social media posts get. 