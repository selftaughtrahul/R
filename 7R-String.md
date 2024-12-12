# String

## String Literals
    Strings are used for storing text.
    A string is surrounded by either single quotation marks, or double quotation marks:
    "hello" is the same as 'hello'

## Assign a String to a Variable
    Assigning a string to a variable is done with the variable followed by the <- operator and the string:

### Examples:

```R
str <- "Hello"
str # print the value of str
```

## Multiline Strings
    You can assign a multiline string to a variable like this:
### Example

```R
str <- "Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."

str # print the value of str
```
#### Note:
    If you want the line breaks to be inserted at the same position as in the code, use the cat() function:
#### Examples
    str <- "Lorem ipsum dolor sit amet,
    consectetur adipiscing elit,
    sed do eiusmod tempor incididunt
    ut labore et dolore magna aliqua."

    cat(str)


## String Length
    There are many useful string functions in R.
    For example, to find the number of characters in a string, use the nchar() function:

### Example:

```R
str <- "Hello World!"
nchar(str)
```
## Check a String
    Use the grepl() function to check if a character or a sequence of characters are present in a string:

### Example:
```R
str <- "Hello World!"

grepl("H", str)
grepl("Hello", str)
grepl("X", str)

```

## Combine Two Strings
    Use the paste() function to merge/concatenate two strings:

### Example:
```R
str1 <- "Hello"
str2 <- "World"
paste(str1, str2)
```

# R Escape Characters

## Escape Characters
    To insert characters that are illegal in a string, you must use an escape character.
    An escape character is a backslash \ followed by the character you want to insert
### Example:
```R
str <- "We are the so-called \"Vikings\", from the north."
str
cat(str)
```

## Other escape characters in R:

| Code   | Result          |
|--------|-----------------|
| `\\`   | Backslash       |
| `\n`   | New Line        |
| `\r`   | Carriage Return |
| `\t`   | Tab             |
| `\b`   | Backspace       |
