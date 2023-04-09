In computer science, an array is a data structure that stores a fixed-size sequential collection of elements of the same type. Each element in an array is identified by an index or a subscript, which represents its position in the array.

In Python, arrays are represented using lists, which are built-in data structures in the language. Here is an example of creating an array in Python using a list:

```Python
# Creating an array of integers
my_array = [1, 2, 3, 4, 5]

# Accessing elements in the array
print(my_array[0])  # Output: 1
print(my_array[2])  # Output: 3

# Changing elements in the array
my_array[0] = 6
print(my_array)  # Output: [6, 2, 3, 4, 5]

# Adding elements to the array
my_array.append(6)
print(my_array)  # Output: [6, 2, 3, 4, 5, 6]

# Removing elements from the array
my_array.remove(2)
print(my_array)  # Output: [6, 3, 4, 5, 6]

# Getting the length of the array
print(len(my_array))  # Output: 5
```

In this example, we create an array of integers using a list called `my_array`. We then access elements in the array using the index, change elements in the array, add elements to the array, and remove elements from the array. Finally, we get the length of the array using the `len()` function.