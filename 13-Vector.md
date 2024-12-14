# Vector
    A Vector is Simply list of iteam that are of the same type.
    to combine the list of item to a vectorm use the

### Example

```R
# Vector of strings
fruits <- c("banana", "apple", "orange")

# Print fruits
fruits

# Vector of numerical values
numbers <- c(1, 2, 3)

# Print numbers
numbers

# To Create A numerical Values  in Sequence
numbers <- 1:10
numbers

# Vector with numerical decimals in a sequence
numbers1 <- 1.5:6.5
numbers1

# Vector with numerical decimals in a sequence where the last element is not used
numbers2 <- 1.5:6.3
numbers2

# Vector of logical values
log_values <- c(TRUE, FALSE, TRUE, FALSE)
log_values

# To find out how many items a vector has, use the length() function:

fruits <- c("banana", "apple", "orange")

length(fruits)

# To sort items in a vector alphabetically or numerically, use the sort() function:

fruits <- c("banana", "apple", "orange", "mango", "lemon")
numbers <- c(13, 3, 5, 7, 20, 2)
sort(fruits)  # Sort a string
sort(numbers) # Sort numbers
```

## Acces Vector
    You can access the vector items by referring to its index number inside brackets []. The first item has index 1, the second item has index 2, and so on

```R
fruits <- c("banana", "apple", "orange", "mango", "lemon")

# Access the first item (banana)
fruits[1]
# You can also access multiple elements by referring to different index positions with the c() function:

# Access the first and third item (banana and orange)

fruits[c(1, 3)]


# You can also use negative index numbers to access all items except the ones specified:

fruits <- c("banana", "apple", "orange", "mango", "lemon")

# Access all items except for the first item
fruits[c(-1)]

```

### Change an Item
    To change the value of a specific item, refer to the index number:


```R
fruits <- c("banana", "apple", "orange", "mango", "lemon")

# Change "banana" to "pear"
fruits[1] <- "pear"

# Print fruits
fruits
```

## Repeat Vectors
    To repeat vectors, use the rep() function:

```R
repeat_each <- rep(c(1,2,3), each = 3)
repeat_each

# Repeat each value independently:
repeat_indepent <- rep(c(1,2,3), times = c(5,2,1))
repeat_indepent

# To make bigger or smaller steps in a sequence, use the seq() function:
numbers <- seq(from = 0, to = 100, by = 20)
numbers

```
#### Note: The seq() function has three parameters: from is where the sequence starts, to is where the sequence stops, and by is the interval of the sequence.
