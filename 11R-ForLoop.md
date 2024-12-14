# For Loops
    A for loop is used for iterating over a sequence:

Example

```R
for (x in 1:10) {
  print(x)
}

fruits <- list("apple", "banana", "cherry")

for (x in fruits) {
  print(x)
}

dice <- c(1, 2, 3, 4, 5, 6)

for (x in dice) {
  print(x)
}

```

# Break
  With the break statement, we can stop the loop before it has looped through all the items:


## Example

```R
fruits <- list("apple", "banana", "cherry")
for (x in fruits) {
  if (x == "cherry") {
    break
  }
  print(x)
}


```
# Next Statements
  With the next statement, we can skip an iteration without terminating the loop:

## Example

```R
fruits <- list("apple", "banana", "cherry")

for (x in fruits) {
  if (x == "banana") {
    next
  }
  print(x)
}

```

