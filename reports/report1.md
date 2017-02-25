# Money "might" buy you some happiness

Does money buy you happiness? It's a decades old question that people have been wondering about. Data seem to suggest that people with high income tend to be happier than people with low income. The analysis on the data suggests that there exists a relationship between the income and happiness level, but the analysis does not provide a substantial evidence that this relationship is a causality. 

Using the data from UChicago NORC's General Social Survey (GSS) on the respondent's income and happiness level, I tried to find whether people with high income are happier than people with low income. Through this question, I tried to gain an insight on whether money has an positive effect on a person's happiness level.

### Methodology

I selected the respondents with high income and low income using the respondent's reported annual household income. For my analysis, I chose the high income group to be people who make up 5th quintile of US annual income level in 2016, which turns out to be about $75,000. The low income group has an income of the bottom quintile of US income level, which is around $17,000. 

For each of the two income groups that I have chosen, I plotted the distribution and calculated the mean of corresponding general happiness value and marriage happiness value. As an additional exploration on the effect of happiness on people's lives, I did the same analysis on the variable that describes how much people value the feeling of accomplishment and importance in their job.

### Results

Following is the probability mass function plot of the distribution of general happiness level for high income and low income group.

![PMF of general happiness level](img/pmf1.png)

The respondents rated their general happiness level using the scale of 1 to 3, 1 being very happy and 3 being not too happy. As you can see from the plot, more fraction of people are happier in the high income group compared to the fraction in the low income group.

To numerically quanitfy the difference in general happiness level for the two groups, I calculated the mean of the happiness values for the each group. Mean happiness value for high income group was about 1.67 while the mean value for the low income group was about 2.00. 

To see whether the income level also affects the marriage happiness, I ran the same analysis on the data of marriage happiness level for the two groups. Following is the PMF plot for the marriage happiness level.

![PMF of marriage happiness level](img/pmf2.png)

The mean marriage happiness value for high income group was about 1.39 while the low income group had a value of 1.5. Like general happiness level, the high income group had lower value than the low income group but the magnitude of difference was much smaller than that of general happiness level.

As an extra, I ran the same analysis on the variable describing the respondent's feeling of accomplishment and importance in the job. The respondents were given five aspects of a job and asked to rank them in order of importance to them. The five choices were job security, number of hours worked, the chance of promotion, the compensation level, and the feeling of accomplishment and importance in the job. Following is the PMF plot of what ranks the respondents gave to the "job importance" aspect.

![PMF of job importance level](img/pmf3.png)

PMF plots of both high income and low income groups were skewed the left, but the plot of high income group was skewed to the left much more. When we calculate the mean, the difference is even more apparent. The mean value for the high income group was about 1.91 while the mean for low income group was about 2.51.

### Interpretation

The mean and the PMF plots of the distribution of general happiness and marriage happiness values present a number of interesting insights. The data suggest that people with high income, categorized as having an annual income that is in the 5th quintile of US annual income, tend to be generally happier in their life and marriage compared to people with low income, with annual income that falls in the 1st quintile of US income. Interestingly, the difference in happiness level between the two groups was much more apparent in the general happiness value than in the marriage happiness value. However, it is worth noting this observation does not provide any substantial evidence of the causality between happiness and income.

Additionally, the data suggest that the people with high income tend to value the feeling of accomplishment and importance of the work in their workplace more than people with low income do.