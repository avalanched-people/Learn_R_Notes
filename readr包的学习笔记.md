# readr包介绍
readr包是R中用于导入文件数据的一个扩展包，成功导入数据的关键是正确解析文件中的文本  
为数据框，因此readr包的功能主要有以下三方面  
**1.  向量的解析——将一个文本向量解析为更加明确的向量类型**  
**2.  列类型的指定——对数据列的类型猜测、指定**  
**3.  矩阵解析——将文件数据转为R语言支持的数据框**    
## 向量解析
`parse_logical()`,`parse_integer()`,`parse_double()`和`parse_character()`是四个最常见的、直接  
用于解析原子向量的函数  
```r
parse_integer(c("1", "2", "3"))
#> [1] 1 2 3 
parse_double(c("1.56", "2.34", "3.56"))
#> [1] 1.56 2.34 3.56
parse_logical(c("true", "false"))
#> [1] TRUE FALSE
```

