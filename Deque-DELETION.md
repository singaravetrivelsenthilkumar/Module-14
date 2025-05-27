# Ex.No:8D Deque - DELETION

## AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

## ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  


## PROGRAM  
```
import collections
a=int(input())
b=int(input())
c=int(input())
de=collections.deque([a,b,c])
de.popleft()
print("The deque after deleting is :")
print(de)
```

## OUTPUT
![Screenshot 2025-05-19 115840](https://github.com/user-attachments/assets/74cd38dc-9381-4727-a06d-cfb0520ba2cd)

## RESULT
Thus a Python program to delete elements at FRONT END of deque using a collection built-in function has been successfully implemented.
