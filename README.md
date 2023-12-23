# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.This code defines two.
2.Functions,linear_search and binary_search.
3.Demonstrates their usebon a sample list(my_list).
4.Linear search checks each element in order.
5.While binary search exploits the sorted nature of find the target element.
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
```python
#Program for linear search method to match the item in a list.
#Developed by:VASANTHARJ J
#RegisterNumber:23012935
def linearSearch(array,n,k):
    for i in range(0,n):
        if (array[i]==k):
            return i
    return  -1
array = eval(input())
k = eval(input())
n=len(array)
array.sort()
result = linearSearch(array,n,k)
if(result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```python
#Program to Find the element in a list using Binary Search(Iterative Method).
#Developed by:VASANTHARJ J
#RegisterNumber:23012935
def BinarySearch(arr , k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if arr[mid]==k:
            return mid
        elif arr[mid]>k:
            return BinarySearch(arr,k,low,mid-1)
        else:
            return BinarySearch(arr,k,mid+1,high)
    else:
            return -1
arr = eval(input())
arr.sort()
k = eval(input())
result=BinarySearch(arr,k,0,len(arr)-1)
if(result==-1):
    print(arr)
    print("Element not found")
else:
    print(arr)
    print("Element found at index: ",result)
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```python
Program to find the element in a list using Binary Search (recursive Method).
Developed by:VASANTHARAJ J
RegisterNumber: 23012935
def BinarySearch(arr, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if arr[mid]==k:
            return mid
        elif arr[mid]>k:
            return BinarySearch(arr,k,low,mid-1)
        else:
            return BinarySearch(arr,k,mid+1,high)
    else:
            return -1
arr = eval(input())
arr.sort()
k = eval(input())
result=BinarySearch(arr,k,0,len(arr)-1)
if(result==-1):
    print(arr)
    print("Element not found")
else:
    print(arr)
    print("Element found at index: ",result)
```
## Sample Input and Output
i)	#Use a linear search method to match the item in a list.
![image](https://github.com/Vasanth2k4/Search-Algorithm/assets/147139769/f1b869d1-a5df-43ea-a528-8e2e513a1a25)

ii)	# Find the element in a list using Binary Search(Iterative Method).
![image](https://github.com/Vasanth2k4/Search-Algorithm/assets/147139769/f0d83f1a-751e-43a9-a83a-84004c4b1566)

iii)	# Find the element in a list using Binary Search (recursive Method).
![image](https://github.com/Vasanth2k4/Search-Algorithm/assets/147139769/d23f32ae-e811-45a1-ad13-c200721b3260)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
