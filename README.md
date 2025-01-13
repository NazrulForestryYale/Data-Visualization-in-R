# Data-Visualization-in-R
This workshop covers commonly used visualization techniques in R.
#Loading packages

library(tidyverse)
library(ggplot2)

#Importing dataset
tree <- read.csv("C:/Users/nazru/OneDrive/Desktop/R Practice/tree.csv")

#Scatter plot
ggplot(data = tree, mapping = aes(x=dbh,y=volume))+
  geom_point()+
  theme_bw()
