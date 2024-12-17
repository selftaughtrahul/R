# The plot() function is used to draw points (markers) in a diagram
    The function takes parameters for specifying points in the diagram.
    Parameter 1 specifies points on the x-axis.
    Parameter 2 specifies points on the y-axis.
## Example
    Draw one point in the diagram, at position (1) and position (3):

```R
plot(1,3)
```

## Draw two points in the diagram, one at position (1, 3) and one in position (8, 10):

```R
plot(c(1, 8), c(3, 10))

```
## multiple Points 
    You can plot as many points as you like, just make sure you have the same number of points in both axis:

```R

plot(c(1, 2, 3, 4, 5), c(3, 7, 8, 9, 12))

```

## For better organization, when you have many values, it is better to use variables:

```R
x <- c(1, 2, 3, 4, 5)
y <- c(3, 7, 8, 9, 12)

plot(x, y)


```

## Sequnce of points 


```R
plot(1:10)

```
## Draw a Line
    The plot() function also takes a type parameter with the value l to draw a line to connect all the points in the diagram

```R
plot(1:10, type="l")

```

## Ploat Labels
    The plot() function also accept other parameters, such as main, xlab and ylab if you want to customize the graph with a main title and different labels for the x and y-axis

```R
plot(1:10, main="My Graph", xlab="The x-axis", ylab="The y axis")
```
## Graph Appearance

```R
plot(1:10, col="red")
```

## Size
Use cex=number to change the size of the points (1 is default, while 0.5 means 50% smaller, and 2 means 100% larger)


```R

plot(1:10, cex=2)

```

## Point Shape
    Use pch with a value from 0 to 25 to change the point shape format:

```R
plot(1:10, pch=25, cex=2)

```

