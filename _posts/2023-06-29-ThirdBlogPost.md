---
title: "Third Blog Post"
author: "Spencer Williams"
date: "2023-06-29"
---

The most interesting thing that I have learned in R so far this semester has been gathering data from an API. In all of my undergrad and graduate classes, we have been given a data set to install from our files. This semester has been my first attempt at trying to get data from an API, and I feel pretty confident after the homework and project. I like how I can search different topics through an API and get specific data from a specific date.

```{r tickers}
library(jsonlite)
outputAPI <- fromJSON("https://api.polygon.io/v3/reference/tickers?active=true&apiKey=BnFt9sqaLWehzloLkpMtEeOG4WjAqkUc")
output <- outputAPI$results
head(output)
```
