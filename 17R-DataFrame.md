# Data Frames in R

Data frames are used to store data in a tabular format. They can hold different types of data in each column. For example, one column can store character data while another can store numeric or logical values. However, within a single column, all values must be of the same type.

---

## Creating a Data Frame
Use the `data.frame()` function to create a data frame:

```R
# Create a data frame
data_frame <- data.frame(
  Training = c("Strength", "Stamina", "Other"),
  Pulse = c(100, 150, 120),
  Duration = c(60, 30, 45)
)

# Print the data frame
data_frame
```

---

## Summarizing Data
Use the `summary()` function to get a summary of the data:

```R
summary(data_frame)
```

---

## Accessing Data Frame Elements
### Access Columns
You can access columns using single brackets `[ ]`, double brackets `[[ ]]`, or the `$` operator:

```R
# Access the first column
data_frame[1]

# Access column by name using double brackets
data_frame[["Training"]]

# Access column by name using the $ operator
data_frame$Training
```

### Access Rows
Use `[row_number, ]` to access a specific row:

```R
# Access the first row
data_frame[1, ]
```

### Access Specific Elements
Use `[row_number, column_number]` to access a specific element:

```R
# Access the element in the first row and second column
data_frame[1, 2]
```

---

## Adding Rows
Use the `rbind()` function to add rows to a data frame:

```R
# Add a new row
new_row_df <- rbind(data_frame, c("Strength", 110, 110))

# Print the updated data frame
new_row_df
```

---

## Adding Columns
Use the `cbind()` function to add columns to a data frame:

```R
# Add a new column
new_col_df <- cbind(data_frame, Steps = c(1000, 6000, 2000))

# Print the updated data frame
new_col_df
```

---

## Removing Rows and Columns
Use the `-` operator with `c()` to remove rows or columns:

```R
# Remove the first row and first column
data_frame_new <- data_frame[-c(1), -c(1)]

# Print the updated data frame
data_frame_new
```

---

## Checking Dimensions
### Number of Rows and Columns
Use the `dim()` function to get both the number of rows and columns:

```R
dim(data_frame)
```

Use `ncol()` to get the number of columns and `nrow()` for rows:

```R
ncol(data_frame)
nrow(data_frame)
```

---

## Data Frame Length
Use the `length()` function to find the number of columns in a data frame (similar to `ncol()`):

```R
length(data_frame)
```

---

## Combining Data Frames
### Combine Vertically
Use the `rbind()` function to combine two or more data frames vertically:

```R
data_frame1 <- data.frame(
  Training = c("Strength", "Stamina", "Other"),
  Pulse = c(100, 150, 120),
  Duration = c(60, 30, 45)
)

data_frame2 <- data.frame(
  Training = c("Stamina", "Stamina", "Strength"),
  Pulse = c(140, 150, 160),
  Duration = c(30, 30, 20)
)

combined_df <- rbind(data_frame1, data_frame2)
combined_df
```

### Combine Horizontally
Use the `cbind()` function to combine two or more data frames horizontally:

```R
data_frame3 <- data.frame(
  Training = c("Strength", "Stamina", "Other"),
  Pulse = c(100, 150, 120),
  Duration = c(60, 30, 45)
)

data_frame4 <- data.frame(
  Steps = c(3000, 6000, 2000),
  Calories = c(300, 400, 300)
)

combined_df2 <- cbind(data_frame3, data_frame4)
combined_df2
