![](https://live.staticflickr.com/65535/55002058152_817b9d1b31_c.jpg)

if missing then we find nearest point on the plane and then fill according the closest point.

Formula used

![](https://live.staticflickr.com/65535/55002948991_22aebdbf49_z.jpg)

weight is the Total number of coordinates/ number of present coordinates

this makes sure we punish those rows whose values are missing, by making their distance longer.

if we we choose k neighbours then k neighbours ki uss value ka mean liya jaega.

while calculating the distance the missing value is ignored.

**Advantages:**

- Very accurate

**Disadvantages:**

- More number of calculations
- Production mei pura training dataset daalna hoga to caculate the missing values for the test data set

# Concept of uniform and distances

Uniform --> for k points --> impute the mean

Distances --> find the values and then reciprocal with distances, to punish those havinng large distances

![](https://live.staticflickr.com/65535/55003137338_a165e5cbc3_c.jpg)

basically jyada paas wale ko jyada weightage do



