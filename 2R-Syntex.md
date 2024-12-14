
# R Syntax

## Outputting Text in R

    To output text in R, you can use single or double quotes:  

```R
"Hello World!"
'Hello World!''
```

# Outputting Numbers in R

    To output numbers, simply type the number without quotes

```R
5
10
```


## Performing Simple Calculations
    You can perform simple calculations by typing expressions directly in R

```R
5 + 8
Output:
[1] 13
```


## Printing Output in R
    Unlike many other programming languages, R can output code without explicitly using a print function

```R
Copy code
"Hello World"
Output:
[1] "Hello World"
```

## Using the print() Function
    R also provides a print() function for output. This function can be useful, especially if you're familiar with other programming languages like Python that often rely on a print() function**

Example:

```R
Copy code
print("Hello World!")
Output:
[1] "Hello World!"
```

## When to Use print()
    There are specific cases where the print() function is required, such as inside loops. For instance, when iterating through a sequence with a for loop

```R
Copy code
for (x in 1:10) {
  print(x)
}
Output:
[1] 1
[1] 2
[1] 3
[1] 4
[1] 5
[1] 6
[1] 7
[1] 8
[1] 9
[1] 10
```

- ## Comments
    Comments can be used to explain R code, and to make it more readable. It can also be used to prevent execution when testing alternative code.
    Comments starts with a #. When executing code, R will ignore anything that starts with #.

This example uses a comment before a line of code:
# This is a comment

```R
 # "Hello World!"
```

## This example uses a comment at the end of a line of code:

```R
"Hello World!" # This is a comment
```


## Multiline Comments
    Unlike other programming languages, such as Java, there are no syntax in R for multiline comments. However, we can just insert a # for each line to create multiline comments:

```R
# written in
# more than just one line
"Hello World!"