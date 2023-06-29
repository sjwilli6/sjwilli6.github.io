Third Blog Post
================
Spencer Williams
2023-06-29

The most interesting thing that I have learned in R so far this semester
has been gathering data from an API. In all of my undergrad and graduate
classes, we have been given a data set to install from our files. This
semester has been my first attempt at trying to get data from an API,
and I feel pretty confident after the homework and project.

``` r
library(jsonlite)
outputAPI <- fromJSON("https://api.polygon.io/v3/reference/tickers?active=true&apiKey=BnFt9sqaLWehzloLkpMtEeOG4WjAqkUc")
output <- outputAPI$results
head(output)
```

    ##   ticker                            name market locale primary_exchange type
    ## 1      A       Agilent Technologies Inc. stocks     us             XNYS   CS
    ## 2     AA               Alcoa Corporation stocks     us             XNYS   CS
    ## 3    AAA AXS First Priority CLO Bond ETF stocks     us             ARCX  ETF
    ## 4  AAAIF        ALTERNATIVE INVSTMENT TR    otc     us             <NA> FUND
    ## 5  AAALF              AAREAL BANK AG AKT    otc     us             <NA>   OS
    ## 6  AAALY         AAREAL BANK AG UNSP/ADR    otc     us             <NA> ADRC
    ##   active currency_name        cik composite_figi share_class_figi
    ## 1   TRUE           usd 0001090872   BBG000C2V3D6     BBG001SCTQY4
    ## 2   TRUE           usd 0001675149   BBG00B3T3HD3     BBG00B3T3HF1
    ## 3   TRUE           usd 0001776878   BBG01B0JRCS6     BBG01B0JRCT5
    ## 4   TRUE           USD       <NA>           <NA>             <NA>
    ## 5   TRUE           USD       <NA>           <NA>             <NA>
    ## 6   TRUE           USD       <NA>   BBG002628DF1     BBG002628F57
    ##           last_updated_utc
    ## 1     2023-06-27T00:00:00Z
    ## 2     2023-06-27T00:00:00Z
    ## 3     2023-06-27T00:00:00Z
    ## 4 2022-08-26T05:00:07.114Z
    ## 5 2022-04-01T06:49:22.884Z
    ## 6 2023-05-04T05:00:29.876Z
