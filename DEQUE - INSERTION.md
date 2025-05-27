# Ex.No:8C DEQUE - INSERTION


## AIM  
To write a Python program to insert elements at REAR END of deque using a collection built-in function.


## ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Initialize an empty deque.  
3. Start an infinite loop using `while True`.  
4. In each iteration, take input from the user.  
5. If the input is an empty string, break the loop.  
6. If the input is not empty, convert it to an integer and append it to the deque.  
7. After the loop ends, append the values `14` and `15` to the deque.  
8. Print the message `"The deque after appending at right is :"`.  
9. Print the contents of the deque.  


## PROGRAM  

```
import collections
a=int(input())
b=int(input())
c=int(input())
de=collections.deque([a,b,c])
de.append(14)
de.append(15)
print("The deque after appending at right is :")
print(de)
```

## OUTPUT
![Screenshot 2025-05-19 115715](https://github.com/user-attachments/assets/7c65accd-de25-4b81-ae81-2a6207bceed9)

## RESULT
Thus a Python program to insert elements at REAR END of deque using a collection built-in function.
