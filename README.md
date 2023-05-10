# wine
Wine data


The matrix plot below is created with the following R code:
---
library(GGally)

    
    ggpairs(data,
        mapping = ggplot2::aes(color = Hue),
        upper = list(continuous = wrap("density", alpha = 0.5), combo = "box_no_facet"))+ggplot2::labs(title = "Wine data")  + 
    theme(axis.text.x = element_text(color="steelblue", 
                                   size=12, angle=90),
        axis.text.y = element_text( color="steelblue", 
                                    size=12))

---

![](https://github.com/NicJC/wine/blob/main/matrixPlot.png)
