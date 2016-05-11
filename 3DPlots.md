# 3DPies
Kamila Kolpashnikova  

# Making 3D Pie Charts

Let's use a package called `plotrix`. First, we need to id the proportions (`slices`) and labels.


```r
library(plotrix)
slices <- c(10, 2, 1, 1, 1)
lbls <- c("School", "Sports", "Intellect", "Drinking", "Profession")
```
 
Now use `pie3D` command to creade your 3D pie chart.


```r
pie3D(slices,labels=lbls,explode=0.2,
      labelrad=1.7,
      main="Topics for Self-esteem")
```

![](3DPlots_files/figure-html/unnamed-chunk-2-1.png) 

You can also change the colors, if you want.


```r
slices1 <- c(2,2, 9)
lbls1 <- c("School", "Food", "Sports")
par(bg = 'white', col='white', col.main='navy', family="Informal Roman")
pie3D(slices1,labels=lbls1,explode=0.2,
      labelrad=1.7, border="mediumpurple3", shade=0.8, 
      col=c("mediumpurple1", "mediumpurple3", "mediumpurple4"),
      main="Topics for Skill Development")
```

![](3DPlots_files/figure-html/unnamed-chunk-3-1.png) 
