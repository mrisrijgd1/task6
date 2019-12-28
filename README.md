# Introduction
This task is from Google Code-In. Here you learn to use the simple Cranlogs API to obtain something. 

# Requirements
- R
- RStudio
- jsonlite
- curl

# Code Description
```
#Task 6

#Use the simple Cranlogs API to obtain half-yearly R package downloads summaries in 2018
library("jsonlite")
#The task is to obtain the total downloads of all R packages in 2018, half-yearly and save the results in a single CSV file
Mridula=jsonlite::fromJSON("https://cranlogs.r-pkg.org/downloads/total/2018-01-01:2018-06-30")
Mridul=jsonlite::fromJSON("https://cranlogs.r-pkg.org/downloads/total/2018-07-01:2018-12-31")
Mriduls=rbind(Mridula, Mridul)
write.csv(Mriduls,"C:\\Users\\srish\\Desktop\\mridul.csv")
```
# Screen Cast
![Record]()

# Authors
- Mridul
