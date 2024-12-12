# R While Loop
    Loops can execute a block of code as long as a specified condition is reached.
    Loops are handy because they save time, reduce errors, and they make code more readable.

## R has two loop commands
   - **while loops**
   -  **for loops**

## 1 R While Loops
    With the while loop we can execute a set of statements as long as a condition is TRUE:

Example
Print i as long as i is less than 6:

```R
i <- 1
while (i < 6) {
  print(i)
  i <- i + 1
}
```
Note: remember to increment i, or else the loop will continue forever.

## Break
    With the break statement, we can stop the loop even if the while condition is TRUE:

```R
Example
Exit the loop if i is equal to 4.

i <- 1
while (i < 6) {
  print(i)
  i <- i + 1
  if (i == 4) {
    break
  }
}
```

## Next
    With the next statement, we can skip an iteration without terminating the loop:


Example
Skip the value of 3:
```R
i <- 0
while (i < 6) {
  i <- i + 1
  if (i == 3) {
    next
  }
  print(i)
}```