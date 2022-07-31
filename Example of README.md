

> dat=mtcars
> pmatrix=scale(dat)
> d=dist(pmatrix)
> c=hclust(d,method="ward.2D")
Error in hclust(d, method = "ward.2D") : 
  invalid clustering method ward.2D
> c=hclust(d, method= "ward.D2")
> plot(c0
+ plot(c)
Error: unexpected symbol in:
"plot(c0
plot"
> plot(c)
> rect.hclust(c,k=4)
> groups<-cutree(c,k=4)
> table(mtcars$Automobiles,groups)
Error in table(mtcars$Automobiles, groups) : 
  all arguments must have the same length
> table(mtcars$Species,groups)
Error in table(mtcars$Species, groups) : 
  all arguments must have the same length
> table(mtcars$cyl,groups)
   groups
     1  2  3  4
  4  0  8  3  0
  6  3  0  4  0
  8  2  0  0 12
> table(mtcars$hp,groups)
     groups
      1 2 3 4
  52  0 1 0 0
  62  0 0 1 0
  65  0 1 0 0
  66  0 2 0 0
  91  0 1 0 0
  93  0 1 0 0
  95  0 0 1 0
  97  0 0 1 0
  105 0 0 1 0
  109 0 1 0 0
  110 2 0 1 0
  113 0 1 0 0
  123 0 0 2 0
  150 0 0 0 2
  175 1 0 0 2
  180 0 0 0 3
  205 0 0 0 1
  215 0 0 0 1
  230 0 0 0 1
  245 0 0 0 2
  264 1 0 0 0
  335 1 0 0 0
