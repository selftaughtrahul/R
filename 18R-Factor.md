# Factors

### Factors are used to categorize data. Examples of factors are:

- **Demography: Male/Female**
-  **Music: Rock, Pop, Classic, Jazz**
- **Training: Strength, Stamina**

To create a factor, use the factor() function and add a vector as argument:

```R
# Create a factor
music_genre <- factor(c("Jazz", "Rock", "Classic", "Classic", "Pop", "Jazz", "Rock", "Jazz"))

# Print the factor
music_genre
```

You can see from the example above that that the factor has four levels (categories): Classic, Jazz, Pop and Rock.

To only print the levels, use the levels() function:


```R

music_genre <- factor(c("Jazz", "Rock", "Classic", "Classic", "Pop", "Jazz", "Rock", "Jazz"))

levels(music_genre)
```

You can also set the levels, by adding the levels argument inside the factor() function:

```R

music_genre <- factor(c("Jazz", "Rock", "Classic", "Classic", "Pop", "Jazz", "Rock", "Jazz"), levels = c("Classic", "Jazz", "Pop", "Rock", "Other"))

levels(music_genre)
```

## Factor Length
Use the length() function to find out how many items there are in the factor:

```R
music_genre <- factor(c("Jazz", "Rock", "Classic", "Classic", "Pop", "Jazz", "Rock", "Jazz"))

length(music_genre)

```

## Access Factors
    To access the items in a factor, refer to the index number, using [] brackets:


```R
music_genre <- factor(c("Jazz", "Rock", "Classic", "Classic", "Pop", "Jazz", "Rock", "Jazz"))

music_genre[3]

```

## Change Item Value
    To change the value of a specific item, refer to the index number:

```R

music_genre <- factor(c("Jazz", "Rock", "Classic", "Classic", "Pop", "Jazz", "Rock", "Jazz"))

music_genre[3] <- "Pop"

music_genre[3]
```
