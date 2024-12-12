# Operators in R
Operators are used to perform operations on variables and values. In the example below, we use the `+` operator to add together two values:

### Example
```R
10 + 5
```

## R divides the operators into the following groups:

- **Arithmetic operators**
- **Assignment operators**
- **Comparison operators**
- **Logical operators**
- **Miscellaneous operators**

---

# 1. Arithmetic Operators
Arithmetic operators are used with numeric values to perform common mathematical operations:

| Operator | Name                | Example    | Try it                     |
|----------|---------------------|------------|----------------------------|
| `+`      | Addition            | `x + y`    | `x <- 5; y <- 3; x + y`    |
| `-`      | Subtraction         | `x - y`    | `x <- 5; y <- 3; x - y`    |
| `*`      | Multiplication      | `x * y`    | `x <- 5; y <- 3; x * y`    |
| `/`      | Division            | `x / y`    | `x <- 5; y <- 3; x / y`    |
| `^`      | Exponentiation      | `x ^ y`    | `x <- 5; y <- 3; x ^ y`    |
| `%%`     | Modulus (Remainder) | `x %% y`   | `x <- 5; y <- 3; x %% y`   |
| `%/%`    | Integer Division    | `x %/% y`  | `x <- 5; y <- 3; x %/% y`  |

---

# 2. Assignment Operators
Assignment operators are used to assign values to variables:

### Examples
```R
my_var <- 3
my_var <<- 3
3 -> my_var
3 ->> my_var
my_var # print my_var
```

**Note:** `<<-` is a global assigner. You will learn more about this in the Global Variable chapter.

It is also possible to reverse the direction of the assignment operator. For example, `x <- 3` is equal to `3 -> x`.

---

# 3. Comparison Operators
Comparison operators are used to compare two values:

| Operator | Name                      | Example     | Try it                     |
|----------|---------------------------|-------------|----------------------------|
| `==`     | Equal                     | `x == y`    | `x <- 5; y <- 3; x == y`   |
| `!=`     | Not equal                 | `x != y`    | `x <- 5; y <- 3; x != y`   |
| `>`      | Greater than              | `x > y`     | `x <- 5; y <- 3; x > y`    |
| `<`      | Less than                 | `x < y`     | `x <- 5; y <- 3; x < y`    |
| `>=`     | Greater than or equal to  | `x >= y`    | `x <- 5; y <- 3; x >= y`   |
| `<=`     | Less than or equal to     | `x <= y`    | `x <- 5; y <- 3; x <= y`   |

---

# 4. Logical Operators
Logical operators are used to combine conditional statements:

| Operator | Description                                                                  |
|----------|------------------------------------------------------------------------------|
| `&`      | Element-wise Logical AND. Returns TRUE if both elements are TRUE            |
| `&&`     | Logical AND. Returns TRUE if both statements are TRUE                       |
| \|     | Element-wise Logical OR. Returns TRUE if one of the statements is TRUE      |
| \|\|    | Logical OR. Returns TRUE if one of the statements is TRUE                   |
| `!`      | Logical NOT. Returns FALSE if the statement is TRUE                         |


---

# 5. Miscellaneous Operators
Miscellaneous operators are used to manipulate data:

| Operator | Description                          | Example                     |
|----------|--------------------------------------|-----------------------------|
| `:`      | Creates a series of numbers in a sequence | `x <- 1:10`               |
| `%in%`   | Checks if an element belongs to a vector | `x %in% y`               |
| `%*%`    | Matrix Multiplication               | `x <- Matrix1 %*% Matrix2` |

