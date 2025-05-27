# Ex.No:8B Circular Queue 

## AIM  
To write a Python program with a function to insert float values into a Circular Queue.


## ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End


## PROGRAM

```
# Queue simply works in FIFO
class Queue:
    def __init__(self, size):
        self.items = [0] * size
        self.max_size = size
        self.head, self.tail, self.size = 0, 0, 0

    def enqueue(self, item):
        if self.is_list_full():
            print(f'Queue is full')
            return

        #print(f'Inserting {item}')
        self.items[self.tail] = item
        self.tail = (self.tail + 1) % self.max_size
        self.size += 1

    def dequeue(self):
        item = self.items[self.head]
        self.head = (self.head + 1) % self.max_size
        self.size -= 1

        return item

    def is_list_full(self):
        if self.size == self.max_size:
            return True
        return False

    def is_empty(self):
        if self.size == 0:
            return True
        return False

size=int(input())
queue = Queue(size)
str=float(input())
str1=float(input())
str2=float(input())
queue.enqueue(str)
queue.enqueue(str1)
queue.enqueue(str2)

    
print(queue.items)
#print(queue.head)
#print(queue.tail)

```

## OUTPUT
![Screenshot 2025-05-19 115517](https://github.com/user-attachments/assets/f766433a-eec3-4c20-92c4-0fb3e77a158e)

## RESULT
Thus a Python program with a function to insert float values into a Circular Queue has been successfully implemenetd.
