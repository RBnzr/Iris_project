library(datasets)
library(tidyverse)
data("iris")

## summary statistics ##

summary(iris)
summary(iris$Sepal.Length)

# check NA

sum(is.na(iris))

install.packages("skimr")

library(skimr)

skim(iris)

#group data by species 

iris %>%
  group_by(Species) %>%
  skim()


## quick data vizualizations
#panel plots

plot(iris)
plot(iris, col = "red")

#scatter plots

plot(iris$Sepal.Width, iris$Sepal.Length, xlab = "Sepal width", ylab = "Sepal lenght" )

#histogram
hist(iris$Sepal.Width)

# feature plot

install.packages(c('caret', 'skimr', 'RANN', 'randomForest', 'fastAdaboost', 'gbm', 'xgboost', 'caretEnsemble', 'C50', 'earth'))
library(carat)

featurePlot(x = iris[,1:4],
            y = iris$Species,
            plot = "box",
            strip = strip.custom(par.strip.text=list(cex=.7)),
            scales = list(x = list(relation="free"),
                          y = list(relation="free")))