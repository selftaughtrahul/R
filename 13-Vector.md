# Vectors in R

Vectors in R are a fundamental data structure that stores elements of the same type, such as numeric, character, or logical.

---

## Creating Vectors
Use the `c()` function to combine items into a vector:

```R
# Vector of strings
fruits <- c("banana", "apple", "orange")
fruits

# Vector of numerical values
numbers <- c(1, 2, 3)
numbers

# Create a sequence of numbers
numbers <- 1:10
numbers

# Create a sequence with decimals
numbers1 <- 1.5:6.5
numbers1

# Create a sequence with decimals where the last element is excluded
numbers2 <- 1.5:6.3
numbers2

# Vector of logical values
log_values <- c(TRUE, FALSE, TRUE, FALSE)
log_values
```

---

## Vector Length
Find out how many elements a vector contains using the `length()` function:

```R
fruits <- c("banana", "apple", "orange")
length(fruits)
```

---

## Sorting Vectors
Sort items in a vector alphabetically or numerically using the `sort()` function:

```R
fruits <- c("banana", "apple", "orange", "mango", "lemon")
numbers <- c(13, 3, 5, 7, 20, 2)

# Sort strings
sort(fruits)

# Sort numbers
sort(numbers)
```

---

## Accessing Vector Elements
Access vector elements by their index inside square brackets `[]`. Indexing starts at 1:

```R
fruits <- c("banana", "apple", "orange", "mango", "lemon")

# Access the first item
fruits[1]

# Access multiple elements
fruits[c(1, 3)]

# Exclude specific elements using negative indexing
fruits[-1]  # Excludes the first element
```

---

## Modifying Vector Elements
Change the value of a specific element by referring to its index:

```R
fruits <- c("banana", "apple", "orange", "mango", "lemon")

# Change "banana" to "pear"
fruits[1] <- "pear"
fruits
```

---

## Repeating Vectors
Repeat elements in a vector using the `rep()` function:

```R
# Repeat each element three times
repeat_each <- rep(c(1, 2, 3), each = 3)
repeat_each

# Repeat elements independently with specified times
repeat_independent <- rep(c(1, 2, 3), times = c(5, 2, 1))
repeat_independent
```

---

## Creating Sequences with Steps
Use the `seq()` function to create sequences with specific intervals:

```R
# Create a sequence from 0 to 100 with steps of 20
numbers <- seq(from = 0, to = 100, by = 20)
numbers
```

### Note
The `seq()` function parameters are:
- `from`: Starting value
- `to`: Ending value
- `by`: Step size

By using vectors, you can efficiently store and manipulate collections of elements in R.
