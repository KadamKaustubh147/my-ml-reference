# Random imputation

This picks random values from the the columnar data and fills the missing value with it

- Preserves variance (since random value imputation hai)
- Memory heavy for deployment (because since columnar data se values impute karna hai toh test mei naya input aaya toh columnar data server pe hona chahiye)
- Well suited for linear models as it does not distort the distribution, regardless of % of NA

# Missing Indicator

We create a new column Named {col_name}_NA, then fill values as true or false, true if missing.


![](https://live.staticflickr.com/65535/55003193975_edd27c6a98_n.jpg)

Some people won a competition and got better accuracy using this method.

just try if and check if it works

![](https://live.staticflickr.com/65535/55002895901_c75b69af9e_c.jpg)

