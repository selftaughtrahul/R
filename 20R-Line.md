# Line Graphics

A line graphic connects all the points in a diagram using a line. To create a line, use the `plot()` function and set the `type` parameter to "l".

## Example
```R
plot(1:10, type = "l")
```

## Line Color
The line color is black by default. To change the color, use the `col` parameter.

```R
plot(1:10, type = "l", col = "blue")
```

## Line Width
To change the width of the line, use the `lwd` parameter (1 is default, while 0.5 means 50% smaller, and 2 means 100% larger).

```R
plot(1:10, type = "l", lwd = 2)
```

## Line Style
The line is solid by default. Use the `lty` parameter with a value from 0 to 6 to specify the line format.

```R
plot(1:10, type = "l", lwd = 5, lty = 3)
```

### Available Parameter Values for `lty`
- **0**: removes the line
- **1**: solid line (default)
- **2**: dashed line
- **3**: dotted line
- **4**: dot-dashed line
- **5**: long-dashed line
- **6**: two-dashed line

## Multiple Lines
To display more than one line in a graph, use the `plot()` function together with the `lines()` function.

```R
line1 <- c(1, 2, 3, 4, 5, 10)
line2 <- c(2, 5, 7, 8, 9, 10)

plot(line1, type = "l", col = "blue")
lines(line2, type = "l", col = "red")
```

