# EXERCISE ALGORITHM
## Exercise 1
### **Reverse string** 

```Python
text = "Hello Baby"
lastIndex = len(text) - 1
reverseText = ""

for index in range(len(text)):
    reverseText += text[lastIndex - index]

print(reverseText)

```
## Exercise 2
### **Reverse string** using a for loop and negative indexing
- reverse a string using a for loop and negative indexing.
```Python
text = "Hello Baby"

reverseText = ""
for index in range(1, len(text) + 1):
    reverseText += text[-index]

print(reverseText)
```
## Exercise 3
### **Count odd munbers**
- checks each element in the list arr and collects the indices of all odd numbers.
```Python
arr = [5, 7, 8, 4, 3]
indexOfOdd = []
for i in range(len(arr)):
    if arr[i] % 2 == 1:
        indexOfOdd.append(i)
print(indexOfOdd)

#Output: [0, 1, 4]
```
## Exercise 4
### **Find Average** of number in list
- calculates the average of the numbers in the list arr by adding them up and dividing the total by how many items are in the list
```Python
arr = [5, 7, 8, 4, 3]
average = 0
sum = 0
for value in arr:
    sum += value
average = sum / len(arr)
print(average)

#Output: 5.4
```
## Exercise 5
### **Access** Array Dictionary
- loops through a list of dictionaries and prints the value associated with the 'name' key for each entry
```Python
arr = [
    {'name': 'bopha', 'age': 18},
    {'name': 'thida', 'age': 12},
    {'name': 'kanha', 'age': 16},
]

for dics in arr:
    print(dics['name'])
```
## Exercise 6
### **Sum** all numbers
- calculates the total sum of all numbers in the array arr
```Python
arr = [5, 7, 8, 4, 3]
sum = 0
for value in arr:
    sum += value
print(sum)

#Output: 27
```
## Exercise 7
### **Count** Even numbers
- loops through the list arr and prints the values that are even
```Python
arr = [5, 7, 8, 4, 3]
for value in arr:
    if value % 2 == 0:
        print(value)

#Output: 8 4
```
## Exercise 8
### **Find** Minimum number in the list
- loop helps you find the smallest number in a list by comparing each element to a reference minimum
```Python
# @Minimum number
arr = [10, 40, 20, 4, 3]
min = arr[0]
for value in arr:
    if value < min:
        min = value
print(min)

#Output: 3
```
## Exercise 9
### **Move** one step to right
- first 1 in the array and moves it one position to the right—just once
```Python
arr = [0, 0, 1, 0, 0]
isFound = False
for i in range(len(arr) - 1):
    if arr[i] == 1 and not isFound:
        arr[i] = 0
        arr[i + 1] = 1
        isFound = True
print(arr)

#Output: [0, 0, 0, 1, 0]
```
## Exercise 10
### **Move** one step to left
- for the first 1 in the array and moves it one step to the left.
```Python
arr = [0, 0, 1, 0, 0]
isFound = False
for i in range(len(arr) - 1):
    if arr[i] == 1 and not isFound:
        arr[i] = 0
        arr[i - 1] = 1
        isFound = True
print(arr)

#Output: [0, 1, 0, 0, 0]
```

## Exercise 11
### **Find** Maximum number in the list
- loop scans through the array and plucks out the largest number.
```Python
arr = [10, 40, 20, 4, 3]
max = arr[0]
for value in arr:
    if value > max:
        max = value
print(max)

#Output: 40
```

## Exercise 12
### **Sum value** in row of Array 2D
- loops through a 2D array and computes the sum of each individual row, storing each result in the arr list
```Python
arr2D = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
]

sum = 0
arr = []
for row in range(len(arr2D)):
    for col in range(len(arr2D[row])):
        sum += arr2D[row][col]
    arr.append(sum)
    sum = 0
print(arr)
```
