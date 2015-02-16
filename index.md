---
title       : International Visitor Arrivals (Singapore)
subtitle    : This application shows the number of travellers taking a trip to Singapore
author      : postalC
job         : Simple Study
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Application Summary

This application shows the total number of visitor arrivals from the world to [Singapore Info](https://www.stb.gov.sg/statistics-and-market-insights/Pages/statistics-visitor-arrivals.aspx) for the range of year(s) selected and their country/region  

The data sources obtained from [Singapore Tourism Board](http://en.wikipedia.org/wiki/Singapore)  

International Visitor Arrivals refer to travellers taking a trip to Singapore whose length of stay is less than a year. For more info visit [Application Site](https://postalc.shinyapps.io/visFull/)  
* All Malaysian citizens arriving by land;  
* Returning Singapore citizens, permanent residents and pass holders;  
* Non-resident air and sea crew (except for sea crew flying in to join a ship); and  
* Air transit and transfer passengers;  
`note` Arrival statistics are reported by country of residence based on information from Disembarkation/ Embarkation (D/E) Cards by the Immigration and Checkpoints Authority of Singapore.  


--- .class #id 

## Data Summary



Structure of Dataset

```
## 'data.frame':	224 obs. of  4 variables:
##  $ Country : Ord.factor w/ 56 levels "Canada"<"USA"<..: 1 2 3 4 5 6 7 8 9 10 ...
##  $ Region  : Ord.factor w/ 8 levels "AMERICAS"<"ASIA (SouthEast)"<..: 1 1 1 2 2 2 2 2 2 2 ...
##  $ Year    : Factor w/ 4 levels "2011","2012",..: 4 4 4 4 4 4 4 4 4 4 ...
##  $ Visitors: num  92.8 484.6 57.5 77.6 3023.1 ...
```

Summary of Visitors Count (in thursands)

```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##     3.6    21.0    56.9   260.0   255.0  3090.0
```

--- .class #id 

## Graph (Visitor Count by Years)

The plot shows the numbers of traveller visited Singapore from 2011-2014 and thier Country or Residence
![plot of chunk graph](figures/graph.png) 

--- .class #id 

## Map (Countries of Residence)
The map shows the scale of traveller number and thier Country of Residence 
![plot of chunk map](figures/map.png) 
