# Project: Analyzing a Market Test



## Step 1: Plan Your Analysis

_To perform the correct analysis, you will need to prepare a data set. (250 word limit)
Answer the following questions to help you plan out your analysis:_

1. What is the performance metric you’ll use to evaluate the results of your test?
    The performance metric that I used to evaluate the results of my test is profit via gross
    margin.
2. What is the test period?
    The test period covers April 29, 2016 till July 21, 2016, which is twelve weeks.
3. At what level (day, week, month, etc.) should the data be aggregated?
    The data should be aggregated at the level of week based on the experiment time.

## Step 2: Clean Up Your Data

_In this step, you should prepare the data for steps 3 and 4. You should aggregate the
transaction data to the appropriate level and filter on the appropriate data ranges. You can
assume that there is no missing, incomplete, duplicate, or dirty data. You’re ready to move on to
the next step when you have weekly transaction data for all stores._ Completed

## Step 3: Match Treatment and Control Units

_In this step, you should create the trend and seasonality variables, and use them along with you
other control variable(s) to match two control units to each treatment unit. Note: Calculate the
number of transactions per store per week to calculate trend and seasonality._

_Apart from trend and seasonality..._

1. What control variables should be considered? Note: Only consider variables in the
    RoundRoastersStore file.
    The control variables that should be consider include the calculated Trend and
    Seasonality among possible others.
2. What is the correlation between your each potential control variable and your
    performance metric?
    By using the Association Analysis tool (see the table below), the correlation between
    each potential control variable (i.e. Sq_Ft and AvgMonthSales) and the performance
    metric (i.e. Gross Margin) showed a strong correlation between AvgMonthSales and
    Gross Margin only (i.e. the correlation between Sq_Ft and Gross Margin is week and
    hence should be ignored).


```
Moreover, for the variable AvgMonthSales the p-value is 0.0000, the correlation is 0.99,
and the statistical significance shows ***. Accordingly, the linear relationship between
AvgMonthSales and Gross Margin is good and verifiable though the scatterplot as
shown below.
```
3. What control variables will you use to match
    treatment and control stores?
    The control variables are used to match treatment
    and control stores via calculating the aggregated
    data of store and the AB Trend tool (see the
    configuration of AB Trend on the right).

```
Hence, by AvgMonthSales, Trend, and Seasonality
as the control variables, each treatment unit is
matched with two control units on a workflow for the
west region and the central region.
```

4. Please fill out the table below with your treatment and control stores pairs:

```
Treatment Store Control Store 1 Control Store 2
2288 2568 9081
2293 12686 9639
2301 12536 9238
2322 9388 3185
2341 2572 12586
1664 1964 7162
1675 7284 2214
1696 1863 7334
1700 7037 2014
1712 8162 7434
```
## Step 4: Analysis and Writeup

_Answer these questions. Be sure to include visualizations from your analysis:_

1. What is your recommendation - Should the company roll out the updated menu to all
    stores?
2. What is the lift from the new menu for West and Central regions (include statistical
    significance)?
3. What is the lift from the new menu overall?

```
A/B analysis is conducted on the west region, central region, and both regions. The
results are shown below:
```
```
Both regions
```
Hence, introducing the new menu in both west and central regions will favorable affect the gross

margin, where 41.9% of average lift would push customers to spend $693.8 more weekly, and

### the significance level of the t-test returns 100%.


```
West region
```
For the west region, introducing the new menu is also profitable and thereby recommended.

The average lift is 37.7% which will increase the profit by $517.7 weekly, and the significance

### level is 99.7%.

```
Central region
```
Nevertheless, the central region reached also good numbers in the analysis and accordingly the

new menu should be introduced. The average lift is 46% that will rise the proft to $869.9 weekly,
and the significance level of t-test is 99.6%.

**Therefore, the recommendation is to introduce the new menu to all stores in both regions**

**to achieve significant profit.**


