# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
## developed by: SIVAKUMAR R
## reg no:212223230209

def linear_search(arr, target):
    for index, item in enumerate(arr):
        if item == target:
            return index
    return -1

input_list = eval(input())
input_list.sort()  
target = int(input())
result = linear_search(input_list, target)
if result != -1:
    print(input_list)
    print(f"Element found at index:  {result}")
else:
    print(input_list)
    print("Element not found")



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
#Developed by:SIVAKUMAR.R
#RegisterNumber:212223230209
def l(arr,b):
    for i in range(len(arr)):
        if arr[i]==b:
            return i
    return -1
arr=eval(input())
b=int(input())
arr.sort()
print(arr)
result=l(arr,b)
if result!=-1:
    print("Element found at index: ",result)
else:
    print("Element not found")
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
# Binary Search (recursive Method).
# Developed by: SIVAKUMAR.R
# RegisterNumber:212223230209
def binary_search_recursive(arr, target, left, right):
    if left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            return binary_search_recursive(arr, target, mid + 1, right)
        else:
            return binary_search_recursive(arr, target, left, mid - 1)
    return -1

arr = eval(input())
target = int(input())
arr.sort()
print(arr)
result = binary_search_recursive(arr, target, 0, len(arr) - 1)
if result != -1:
    print("Element found at index: ", result)
else:
    print("Element not found")
```
## Sample Input and Output
![Screenshot 2024-05-10 182327](https://github.com/SIVAmech123/Search-Algorithms/assets/151629067/c1c5ee1c-5285-41d4-bb68-243de9df08ab)

![Screenshot 2024-05-10 182334](https://github.com/SIVAmech123/Search-Algorithms/assets/151629067/0ab4a10f-4bf0-465f-9f56-8aea6792a96e)

![Screenshot 2024-05-10 182342](https://github.com/SIVAmech123/Search-Algorithms/assets/151629067/3b224f5a-f374-4a7c-8ff7-1297e073034a)
![Screenshot 2024-05-10 182347](https://github.com/SIVAmech123/Search-Algorithms/assets/151629067/57bd08c7-ae65-4181-a328-420f7bf0c163)
![Screenshot 2024-05-10 182356](https://github.com/SIVAmech123/Search-Algorithms/assets/151629067/38c9f185-f14f-4c17-a7d8-7d3df5fce19b)

![Screenshot 2024-05-10 182401](https://github.com/SIVAmech123/Search-Algorithms/assets/151629067/fcc94e21-1266-457a-980a-f73ed3db3733)



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
