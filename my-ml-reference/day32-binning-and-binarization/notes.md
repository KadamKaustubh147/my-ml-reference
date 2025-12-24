# Notes

Sometimes we may want to encode numerical data to categorical data.

But why?

Lets say we have a dataset of apps, and there is a column of number of downloads.

and differnt apps have diffrent no. of downloads like 23, 200k, 1M etc.

Now since these numbers could be easily grouped in range we do it that way.

---

## There are two ways to encode numerical data to categorical data.

1. Discretization (Binning)
2. Binarisation

### Binnning/Discretization

We make ranges or bins like a histogram/

![](https://live.staticflickr.com/65535/54999389846_5c0e6fc67b_z.jpg)

#### Types of binning

![](https://live.staticflickr.com/65535/54998511572_b782128252.jpg)

#### 1.  Unsupervised binning

- Equal width (uniform)
- Equal frequency (Quantile)
- KMeans binning

##### Equal width/Uniform binning

You have to specify the number of bins

Now 

![](https://live.staticflickr.com/65535/54998521942_cc0faf0a25_z.jpg)

The width is equal

1. Great for handling outliers
2. No change in spread

##### Equal frequency (Quantile)

Specify the number of bins

Bins are based on frequency not width

![](https://live.staticflickr.com/65535/54999721050_85aa3faede_z.jpg)

This also handles:

1. Outliers
2. makes the spread uniform

![](https://live.staticflickr.com/65535/54998528062_d8184741ec_w.jpg)

This used frequently

##### KMeans Binning

When the data is in cluster.

We specify the bins

Algo

1. We specify random centroids first
2. Now we calculate random distances from each point to that centroid and divide the data into clusters
3. Like ek point jiss centroid ke paas hai voh uss cluster mei jaega
4. Now we change the centroid --> by taking mean i.e the new mean is the new centroid
5. and we repeat

![](https://live.staticflickr.com/65535/54999737490_520e53d806_b.jpg)
![](https://live.staticflickr.com/65535/54999693394_f19626c4b1.jpg)

![](https://live.staticflickr.com/65535/54999431366_1672884d69_b.jpg)

#### 2.  Custom binning

Custom binning -> make custom binning (not available in sklearn ig need to use pandas for this)

Bins like this

![](https://live.staticflickr.com/65535/54998561107_e5a212105d_w.jpg)

#### 3.  Supervised binning

- Decision Tree binning

(This is rare and requires decision tree as prerequsite)


### Binarisation

Niche technique

In image processing lets say we want to change an image to black and white.

so the rgb value of the pixel is from 0-255

so less than 127.55 the value of the pixel is 0
and greater than 127.5 the value of the pixel is 1

