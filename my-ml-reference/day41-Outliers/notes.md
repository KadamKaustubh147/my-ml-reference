# What are outliers

Outliers are the extremeties of the data.

for a column outlier is that data that will show extremeties

A ML model gets distracted due to outliers

for example

![](https://live.staticflickr.com/65535/55003464033_eb3d7bec63_m.jpg)

the first line is due to outliers --> inaccurate line

second line is the accurate line

# When are outliers dangerous and we should remove them?

Lets say age is 300 --> physically impossible --> therfore remove it

but lets say you are doing anomaly detection for network or for credit card fraud detection.

Then we have to keep outliers.

Now in the above graph we see there are two axes marks and hours.

we can also do that instead of removing outliers we 


# Effects of outliers in ML algos

- Linear regression
- Logistic regression
- Adaboost
- Deep learning

If weight based algo --> outliers affect it

tree based algos don't get affected by outliers.

# How to treat outliers

1. trimming --> directly remove kardo --> very fast
2. Capping --> replace with max and min (like in IQR for skewed and mean+3*s.d)
3. Replace with Missing values --> and use old techniques
4. Do discretisation --> like encoding numerical data into categorical data

# How to detect outliers

1. If distribution is normally distributed

![](https://live.staticflickr.com/65535/55003627370_5a102bdec7_w.jpg)

mean +/- 3*s.d is the maximum and minimum outside this is outlier

2. for skewed distribution

IQR = Q3-Q1

Q3 + 1.5*IQR --> maximum

Q1 - 1.5*IQR --> minimum

outside of this maximum and minimum range is outlier.

3. For other distributions we can use percentile based system

![](https://live.staticflickr.com/65535/55003444206_cbe9895bf9.jpg)



# techniques for outlier removal

![](https://live.staticflickr.com/65535/55003445786_8601b795d2_z.jpg)

for removal in normal distribution --> we use z-score..

