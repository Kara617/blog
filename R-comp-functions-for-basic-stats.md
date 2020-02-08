## R Functions for Basic Statistics  
**Basic Graphs** | **Basic R** | **ggplot2**
-----------------|-------------|---------
histogram 直方图  |    hist    | geom_histogram  


### <font color = "purple">Histogram 直方图</font>  
直方图能够概括数据得分布  

**1. Making a Basic Histogram**  
geom_histogram(mapping = NULL, data = NULL, stat = "bin",
  position = "stack", ..., binwidth = NULL, bins = NULL,
  na.rm = FALSE, show.legend = NA, inherit.aes = TRUE)  
可视化单个连续性变量  

> Visualise the distribution of a single continuous variable by dividing the x axis into bins and counting the number of observations in each bin.   

Histograms(`geom_histogram()`) display the counts with **bars**  

```r
ggplot(diamonds, aes(carat)) +
  geom_histogram(binwidth = 0.01)
```

**参数binwidth**  
![]("D:/SJTU/研一课程/统计软件R/ISLR/hist-binwidth.png")
