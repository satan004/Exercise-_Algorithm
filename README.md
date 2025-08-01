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

```Python
text = "Hello Baby"

reverseText = ""
for index in range(1, len(text) + 1):
    reverseText += text[-index]

print(reverseText)
```
## Exercise 3
### **Count odd munbers**
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
```Python
arr = [5, 7, 8, 4, 3]
for value in arr:
    if value % 2 == 0:
        print(value)

#Output: 8 4
```
## Exercise 8
### **Find** Minimum number in the list
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
