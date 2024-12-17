# Scatter Plots
A "scatter plot" is a type of plot used to display the relationship between two numerical variables, and plots one dot for each observation.

## Example 1: Basic Scatter Plot

```R
# Example 1: Basic Scatter Plot
x <- c(5, 7, 8, 7, 2, 2, 9, 4, 11, 12, 9, 6)
y <- c(99, 86, 87, 88, 111, 103, 87, 94, 78, 77, 85, 86)

plot(x, y)
```

### Description
The plot in the example above shows the observation of 12 cars passing by. Each dot represents a car, with its age (`x`) and speed (`y`) plotted against each other.

## Example 2: Scatter Plot with Titles and Labels

```R
x <- c(5, 7, 8, 7, 2, 2, 9, 4, 11, 12, 9, 6)
y <- c(99, 86, 87, 88, 111, 103, 87, 94, 78, 77, 85, 86)

plot(x, y, main="Observation of Cars", xlab="Car Age", ylab="Car Speed")
```

### Description
This example includes a title and axis labels to provide more context about the data being plotted. The `main` argument sets the title, `xlab` labels the x-axis, and `ylab` labels the y-axis.

## Example 3: Comparing Two Sets of Observations

To compare the plot with another dataset, use the `points()` function to overlay the additional data on the same plot:

```R
# Day one: the age and speed of 12 cars
x1 <- c(5, 7, 8, 7, 2, 2, 9, 4, 11, 12, 9, 6)
y1 <- c(99, 86, 87, 88, 111, 103, 87, 94, 78, 77, 85, 86)

# Day two: the age and speed of 15 cars
x2 <- c(2, 2, 8, 1, 15, 8, 12, 9, 7, 3, 11, 4, 7, 14, 12)
y2 <- c(100, 105, 84, 105, 90, 99, 90, 95, 94, 100, 79, 112, 91, 80, 85)

# Plot day one data
plot(x1, y1, main="Observation of Cars", xlab="Car Age", ylab="Car Speed", col="red", cex=2)

# Overlay day two data
points(x2, y2, col="blue", cex=2)
```

### Description
- `plot()` is used to create the initial scatter plot for day one, with red points.
- `points()` overlays the scatter plot for day two, with blue points.
- The `cex` parameter adjusts the size of the points.

This visualization allows comparison between the two datasets on the same axes.

