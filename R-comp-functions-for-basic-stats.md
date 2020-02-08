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
![img](https://github.com/Kara617/blog/blob/master/R-graphs/hist-binwidth.png)

**参数binwidth & bins**  
* 条形宽度 binwidth: The width of the bins.  
* 条形个数 bins: overridden by `binwidth`; Default to 30  

```r
ggplot(diamonds, aes(carat)) +
  geom_histogram(bins = 200)
```
