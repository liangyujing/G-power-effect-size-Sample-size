# descriptive
# 1. descriptive statistics

#gender ratio
table(gender)

#mean, sd
aggregate(antisemitism_07, list(liedetection,suffering),mean)
aggregate(antisemitism_07, list(liedetection,suffering), SD)


#install.packages("psych")
library(psych)
describe(antisemitism_07,fast=TRUE)  
