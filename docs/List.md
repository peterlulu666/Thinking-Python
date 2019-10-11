# List      

A list is a sequence of values. The first index is 0.      

List is mutable. We would change the element is the list. `list.append(value)` `list.pop(index)` `list.remove(value)`.      

Copying a list      

```python
a = [1, 2, 3]      
b = a 
```     

The list `a` and `b` is referencing to the same address of memory. If you modify `a`, you are changing `b`.            

```python
a = [1, 2, 3]
b = []
for item in a:
    b.append(item)

```      

The list `a` and `b` is referencing to the different address of memory.        







      






       









         

















