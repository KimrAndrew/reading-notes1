# NumPy is a commonly used Python data analysis package

## Numpy 2-Dimensional Arrays

  - known as a matrix
  - list of lists
  - has rows and columns
  - extract inforamtion using rows and columns

## Creating a NumPy Array

`numpy.array`
  - if passed a list of lists, automatically creates a NumPy array
  - all elements in the array need to be of the same type

`array.shape`
  - returns a tuple with number of rows and columns

## Using NumPy To Read In Files

`numpy.genfromtxt`
  - passed a file
  - delimeter
  - skip_header

## Indexing NumPy Arrays
  - [row,column]

Numpy Array Operations

## Single Array Math

- basic math operators performed on an array will apply the operation to each element in the array

## Multiple Array Math

- applies the operation to pairs of elements
- column-to-column

## Broadcasting
  - The last dimension of each array is compared
    - checks if lengths are equal or if one dimension is of length 1
    - if neither throws an error
