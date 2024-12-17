# Pie Chart
A pie chart is a circular graphical view of data, used to represent proportions or percentages among categories.

## Example

```R
# Create a vector of pies
x <- c(10, 20, 30, 40)

# Display the pie chart
pie(x)
```

## Start Angle
You can change the start angle of the pie chart with the `init.angle` parameter. The value of `init.angle` is specified in degrees, where the default angle is 0.

```R
# Create a vector of pies
x <- c(10, 20, 30, 40)

# Display the pie chart and start the first pie at 90 degrees
pie(x, init.angle = 90)
```

## Labels and Header
Use the `labels` parameter to add labels to the pie chart, and use the `main` parameter to add a header.

```R
# Create a vector of pies
x <- c(10, 20, 30, 40)

# Create a vector of labels
mylabel <- c("Apples", "Bananas", "Cherries", "Dates")

# Display the pie chart with labels
pie(x, labels = mylabel, main = "Fruits")
```

## Colors
You can add colors to each pie slice using the `col` parameter.

```R
# Create a vector of colors
colors <- c("blue", "yellow", "green", "black")

# Display the pie chart with colors
pie(x, labels = mylabel, main = "Fruits", col = colors)
```

## Legend
To add a legend explaining each pie slice, use the `legend()` function.

```R
# Create a vector of labels
mylabel <- c("Apples", "Bananas", "Cherries", "Dates")

# Create a vector of colors
colors <- c("blue", "yellow", "green", "black")

# Display the pie chart with colors
pie(x, labels = mylabel, main = "Pie Chart", col = colors)

# Display the legend
legend("bottomright", mylabel, fill = colors)
```

### Legend Positions
The legend can be positioned using the following keywords:
- `bottomright`
- `bottom`
- `bottomleft`
- `left`
- `topleft`
- `top`
- `topright`
- `right`
- `center`

Choose the position based on your preferred layout and visibility requirements.

