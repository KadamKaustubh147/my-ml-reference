# Multivariate imputation technique 2

> MICE

again dicussing 3 types of missing data

MCAR --> missing completely at random

MAR --> Missing at random

MNAR --> Missing not at random (jan bujh ke gayab kiya hai)

MAR is like missing at random but for some reason

like age or weight nai fill kiya kyuki optional hai.

Now thru other columns we can fill/predict the missing data

---

MICE

![](https://live.staticflickr.com/65535/55003298560_c672202a8a_n.jpg)

Slow because it uses a ML algo to predict your values (literally)

Algo

1. We pick a column to fill the missing data.
2. For the other columns we do mean imputation
3. Now we apply any ML(LR, decision tree etc.) and predict the missing values

![](https://live.staticflickr.com/65535/55003267829_15242dd082_b.jpg)

![](https://live.staticflickr.com/65535/55002121542_f4c404dab7_b.jpg)

now we do this for all the columns

4. We start again from column and do it n times (depending on number of iterations)
5. Now we take Iteration 0 and Iteration 2 and find the difference


![](https://live.staticflickr.com/65535/55003273184_6bd0dc634b_b.jpg)


we do the iterations till the difference does not become close to 0.

or for a fixed number of iterations
