# Lists in R

Lists in R can contain elements of different data types, such as strings, numbers, vectors, and other lists. A list is ordered and mutable.

---

## Creating Lists
Use the `list()` function to create a list:

```R
# List of strings
this_list <- list("apple", "banana", "cherry")

# Print the list
this_list
```

---

## Accessing List Elements
List items can be accessed using their index inside double square brackets `[[ ]]` or with single brackets `[ ]` for sub-lists.

```R
this_list <- list("apple", "banana", "cherry")

# Access the first item
this_list[[1]]

# Access a sub-list
this_list[1]
```

---

## Modifying List Elements
You can change the value of a specific item by referring to its index:

```R
this_list <- list("apple", "banana", "cherry")

# Change the first item
this_list[[1]] <- "blackcurrant"

# Print the updated list
this_list
```

---

## List Length
Find the number of elements in a list using the `length()` function:

```R
this_list <- list("apple", "banana", "cherry")

length(this_list)
```

---

## Checking for Item Existence
Use the `%in%` operator to check if a specific item exists in a list:

```R
this_list <- list("apple", "banana", "cherry")

"apple" %in% this_list
```

---

## Adding Items to a List
Use the `append()` function to add items to a list:

```R
this_list <- list("apple", "banana", "cherry")

# Add an item to the end of the list
this_list <- append(this_list, "orange")

# Add an item after a specific position
this_list <- append(this_list, "orange", after = 2)
```

---

## Removing Items from a List
Remove items by creating a new list without the unwanted elements:

```R
this_list <- list("apple", "banana", "cherry")

# Remove the first item
new_list <- this_list[-1]

# Print the new list
new_list
```

---

## Slicing a List
Access a range of items using indexing:

```R
this_list <- list("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")

# Access items from index 2 to 5
this_list[2:5]
```

---

## Joining Lists
Combine two or more lists using the `c()` function:

```R
list1 <- list("a", "b", "c")
list2 <- list(1, 2, 3)

# Join lists
combined_list <- c(list1, list2)

# Print the combined list
combined_list
```

By using lists, you can store and manipulate heterogeneous data in R efficiently.
