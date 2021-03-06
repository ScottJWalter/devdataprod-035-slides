Developing Data Products
========================================================
author: Scott Walter
date: Sun Dec 27 12:30:43 2015

Description
========================================================

This project is a simple Shiny application that looks at the USDA
Food Environment Atlas data, located at:

http://www.ers.usda.gov/data-products/food-environment-atlas/data-access-and-documentation-downloads.aspx

Description
========================================================
It allows the user to view various data points within
the `STORES` subset of data:

- Grocery Stores
- Supercenters & club stores
- Convenience stores
- Specialized food stores

And see the differences between data collected in 2007 and 2012, as
well as the difference betwen the two sets.

Example Execution
========================================================

The application allows you to select the data point to view,
then plots it:


```r
# load the data set
source("init.R")

# plot an example graph
plot(
    df[["State"]]
    , df[["Grocery stores (% change), 2007-12"]]
    , main = paste("Grocery stores (% change), 2007-12", "by State")
    , xlab = "State"
    , ylab = "Grocery stores (% change), 2007-12"
)
```

Example Plot
========================================================

![plot of chunk unnamed-chunk-2](devdataprod-035-figure/unnamed-chunk-2-1.png) 
