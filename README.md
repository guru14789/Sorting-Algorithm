# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
# Program to sort the elements in the list using the Selection Sort algorithm.
# Developed by:SREEKUMAR S
# RegisterNumber: 23008070

def selection_sort(arr):
    n=len(arr)
    for i in range(n-1):
        index=i
        for j in range(i+1,n):
            if arr[j]<arr[index]:
                index=j
        arr[i],arr[index]=arr[index],arr[i]
    return arr
        


arr= eval(input())
print(selection_sort(arr))
```
ii)	#Insertion Sort
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by:SREEKUMAR S
RegisterNumber: 23008070

def insertion_sort(arr):
    for i in range(1,len(arr)):
        a=arr[i]
        j=i-1
        
        while j>=0 and a<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=a
    return arr

    
    
arr= eval(input())
print(insertion_sort(arr))
```

## Output:
![case1 sort](https://github.com/guru14789/Sorting-Algorithm/assets/151705853/f75acc5c-451a-4292-a7c6-c97202241b90)
![case 2 sort](https://github.com/guru14789/Sorting-Algorithm/assets/151705853/2c79a76d-bb92-45fd-aaf5-e63506f2d21c)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
