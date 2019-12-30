# 这是一些学习ggplot的笔记，个人整理一下，以便查看复习  
安装与加载ggplot2包  
```r
install.packages(ggplot2)
library(ggplot2)
```
ggplot函数的基本语法结构：  
```r
ggplot(data = mpg, aes(x = displ, y = hwy)) +
  geom_point()
```
在ggplot中，放在aes()中表示其中的数据需要经过美学映射，放在aes外面则不需要,比如：  
```r
ggplot(data = mpg, aes(x = displ, y = hwy), colour = "red")) +
  geom_point()
```
和  
```r
ggplot(data = mpg, aes(x = disp, y = hwy, colour = "red")) + 
  geom_point()
```
这两者是不一样的，在aes()函数中会产生一个变量名为red，而后采用默认的颜色粉红色（pinkish）点图  
在aes()函数外，则会直接绘制红色的点图  
这一点需要牢记  










