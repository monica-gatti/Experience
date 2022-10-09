
# PYTHON DATA STRUCTURES
Python doesn't have a built-in type for matrices. However, we can treat a list of a list as a matrix.
Python provides 4 built-in data types in Python used to store collections of data
- List
- Tuple
- Set
- Dictionary
all with different qualities and usage.

## List
List items are ordered, changeable, and allow duplicate values.
List items are indexed, the first item has index [0], the second item has index [1]
Lists are used to store multiple items in a single variable.
When we say that lists are ordered, it means that the items have a defined order, and that order will not change.
If you add new items to a list, the new items will be placed at the end of the list. 
The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.
Lists allow duplicate values.
Lists are created using square brackets:
```
from typing import Tuple
A = [[1, 4, 5, 12],
    [-5, 8, 9, 0],
    [-6, 7, 11, 19]]
print("A =", A)
print("A[1] =", A[1])      # 2nd row
print("A[1][2] =", A[1][2])   # 3rd element of 2nd row
print("A[0][-1] =", A[0][-1])   # Last element of 1st Row

column = [];        # empty list
for row in A:
  column.append(row[2])  

print("3rd column =", column)
```

# Program to add two matrices using nested loop

```
X = [[12,7,3],
    [4 ,5,6],
    [7 ,8,9]]

Y = [[5,8,1],
    [6,7,3],
    [4,5,9]]

result = [[0,0,0],
          [0,0,0],
          [0,0,0]]

def matrixaddition(A1, A2, result):
  for i in range(len(X)):
    for y in range(len(X)):
      result[i][y] = X[i][y] + Y[i][y]

matrixaddition(X, Y, result)
print(result)
```

# Program to add two matrices using list comprehension
````
result = [[X[i][j] + Y[i][j]  for j in range(len(X[0]))] for i in range(len(X))]
print("Program to add two matrices using list comprehension")
for r in result:
   print(r)
```
  
## Tuple
Tuple items are ordered, unchangeable, and allow duplicate values.
Tuple items are indexed, the first item has index [0], the second item has index [1] etc.
Tuples are unchangeable, meaning that we cannot change, add or remove items after the tuple has been created.
When we say that tuples are ordered, it means that the items have a defined order, and that order will not change.
```
tupla = ("a1", "a2", "a4")
print(tupla[1])


## Set
A set is a collection which is unordered, unchangeable*, and unindexed.
Set items are unchangeable, but you can remove items and add new items.
Duplicates are not allowed
```
myset = {"u1", "u2", "u3" ,"u4"}
myset.add("k4")
print(myset)

thisset = {"apple", "banana", "cherry"}

for x in thisset:
  print(x)
```

## Dictionary
```
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
```
