# Stacks-n-Queues

## Intro

Stacks and queues are two data structures that access and handle data in similar, but distinctly different, ways. Queues act as a line. The first thing, or pieces of data, to enter the queue, are the first to be executed, or exit the line (first in, first out, or "FIFO"). Stacks on the other hand, are a pile. Whatever has been placed on top, must be the first to be removed, or executed, before the rest of the stack can be executed (last in, first out, or "LIFO"). Be sure not to 'stack' the pile too high, or the whole thing could topple. THIS IS STACK OVERFLOW! GET IT!? DO YOU GET IT!?!?!?!?!?!?<br/>
![](https://4cawmi2va33i3w6dek1d7y1m-wpengine.netdna-ssl.com/wp-content/uploads/2018/07/Computer-science-fundamentals_6.1.png)

## Examples

Imagine you wanted to get a pair of sneakers. There are two different stores that you can get to easily. One store, like most stores, will tell people to stand in the line OR QUEUE and wait to enter. The first in line will be the first to enter the store and be able to make their purchase. Last in, first out. The second store on the other hand, is holding a sort of contest. They're challenging anyone who wants a pair of these sneakers to game of king of the hill (OR STACK). Whoever is the last woman standing on top of the hill will be the one selected to be able to make their purchase.

A more technical/computery example of a queue would be the way that computer processing unit (CPU) scheduling is based on a queue. Tasks are executed in the order in which they were called, while the execution of tasks further down in the queue is put on hold until resources are available.

And to round this out with a technical/computery example of a stack; the "back" button on your browser is an excellent one. As you browse, the urls that you visit are saved in a stack. When you navigate with the "forward" or "back" buttons, you're navigating up and down through that stack.

## Queue implementation in Python
# Assign Queue to class
class Queue:
    def __init__(self):
        self.queue = []
# Add an element
   def enqueue(self, item):
        self.queue.append(item)
# Remove an element
   def dequeue(self):
        if len(self.queue) < 1:
            return None
        return self.queue.pop(0)
# Display  the queue
   def display(self):
        print(self.queue)
    def size(self):
        return len(self.queue)
q = Queue()
q.enqueue(1)
q.enqueue(2)
q.enqueue(3)
q.enqueue(4)
q.enqueue(5)
q.display()
q.dequeue()
print("After removing an element")
q.display()
<br/>
## Stack implementation in Python
# Append an element
>>> myStack = []
>>> myStack.append('a')
>>> myStack.append('b')
>>> myStack.append('c')
# Display the stack
>>> myStack
['a', 'b', 'c']
# Pop an element
>>> myStack.pop()
'c'
>>> myStack.pop()
'b'
>>> myStack.pop()
'a'
>>> myStack.pop()
Traceback (most recent call last):
  File "<console>", line 1, in <module>
IndexError: pop from empty list

## Potential Questions

Q: Let's say that you want to build a social media app like instagram. Your intention is to be able have users post images with text attached to them, and then display those post so that the most recent would always be at the top. What data structure would you use to display these posts?

A: Stack. The last thing that was posted, should be the first seen. LIFO BABY!

Q: Now let's say that you wanted to create a recipe app. Your design calls for a component on your home page that will always display only the 10 most recent recipes that were posted, in the order they were posted. Which data structure should you use?

A: Queue. The earliest recipes, or the first ones added, should be removed as new recipes are added. That's a little FIFO for you. Bring it home to your mother so she can hang it on the fridge.

[Take a look to learn more](https://everythingcomputerscience.com/discrete_mathematics/Stacks_and_Queues.html)<br/>
[This video is great for you visual learners](https://www.youtube.com/watch?v=wjI1WNcIntg)
