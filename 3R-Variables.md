# Creating Variables in R

R is a dynamically typed language, meaning you don't need to declare a variable's data type before assigning a value. The <- operator is commonly used to assign values to variables.

Example:

## Creating numeric, character, and logical variables
```R
x <- 10  # Numeric
y <- "Hello, world!"  # Character
z <- TRUE  # Logical

```
Concatenating Elements
To combine strings or variables into a single string, use the paste() function. It takes multiple arguments and concatenates them, separating them with a specified separator.

Example:

Code snippet

```R
first_name <- "Alice"
last_name <- "Wonderland"
```

## Concatenate with a space separator

```R full_name <- paste(first_name, last_name)
print(full_name)  # Output: "Alice Wonderland"
```

## Concatenate with a custom separator

```R
message <- paste("Hello,", first_name, "from", last_name, sep=" ")
print(message)  # Output: "Hello, Alice from Wonderland"
```

## You can also use , to add a variable to another variable

```R
text1 <- "R is"
text2 <- "awesome"

paste(text1, text2)

```

## For numbers, the + character works as a mathematical operator

```R
num1 <- 5
num2 <- 10
print(num1 + num2)

```

## R Multiple Variables

## R allows you to assign the same value to multiple variables in one line

```R
var1 <- var2 <- var3 <- "Orange"
# Print variable values
var1
var2
var3
```

## R Variable Names (Identifiers)

'''Variable Names
A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for R variables are:
A variable name must start with a letter and can be a combination of letters, digits, period(.)
and underscore(_). If it starts with period(.), it cannot be followed by a digit.
A variable name cannot start with a number or underscore (_)
Variable names are case-sensitive (age, Age and AGE are three different variables)
Reserved words cannot be used as variables (TRUE, FALSE, NULL, if...)'''

# Legal variable names

myvar <- "John"
my_var <- "John"
myVar <- "John"
MYVAR <- "John"
myvar2 <- "John"
.myvar <- "John"

# Illegal variable names

2myvar <- "John"
my-var <- "John"
my var <- "John"
_my_var <- "John"
my_v@ar <- "John"
TRUE <- "John"
