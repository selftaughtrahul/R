# R If ... Else
    Conditions and If Statements

## R supports the usual logical conditions from mathematics:

| Operator | Name                      | Example      | Try it   |
|----------|---------------------------|--------------|----------|
| `==`     | Equal                     | `x == y`     |          |
| `!=`     | Not equal                 | `x != y`     |          |
| `>`      | Greater than              | `x > y`      |          |
| `<`      | Less than                 | `x < y`      |          |
| `>=`     | Greater than or equal to  | `x >= y`     |          |
| `<=`     | Less than or equal to     | `x <= y`     |          |


## The if Statement
    An "if statement" is written with the if keyword, and it is used to specify a block of code to be executed if a condition is TRUE:

Examples:
```R
a <- 33
b <- 200

if (b > a) {
  print("b is greater than a")
}

```

Note R uses curly brackets { } to define the scope in the code.

## Else If
    The else if keyword is R's way of saying "if the previous conditions were not true, then try this condition":

Example
```R
a <- 33
b <- 33

if (b > a) {
  print("b is greater than a")
} else if (a == b) {
  print ("a and b are equal")
}
```

## If Else
    The else if keyword is R's way of saying "if the previous conditions were not true, then try this condition":

Example

```R
a <- 33
b <- 33

if (b > a) {
  print("b is greater than a")
} else if (a == b) {
  print ("a and b are equal")
}
```


# R Nested If
    You can also have if statements inside if statements, this is called nested if statements.

Example

```R
x <- 41

if (x > 10) {
  print("Above ten")
  if (x > 20) {
    print("and also above 20!")
  } else {
    print("but not above 20.")
  }
} else {
  print("below 10.")
}
```

# R - AND OR Operators
    The & symbol (and) is a logical operator, and is used to combine conditional statements:

Example

```R
Test if a is greater than b, AND if c is greater than a:

a <- 200
b <- 33
c <- 500

if (a > b & c > a) {
  print("Both conditions are true")
}
```

## OR
    The | symbol (or) is a logical operator, and is used to combine conditional statements:

Example
```R
Test if a is greater than b, or if c is greater than a:

a <- 200
b <- 33
c <- 500

if (a > b | a > c) {
  print("At least one of the conditions is true")
}
```