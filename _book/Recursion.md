# Recursion and dictionary

## Recursion

A function that calls itself is recursive.

## Dictionary

We would use `dict()` to create the dictionary.

We would add items to the dictionary. `eng2sp["key"] = "value"`.

We would create a dictionary with three items.

`eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}`.



```python
eng2sp = dict()
eng2sp["one"] = "uno"
print(eng2sp)
eng2sp = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
print(eng2sp)
print(eng2sp["three"])

```

> **[info] Dictionary**
* The output would be `{'one': 'uno'}`, `{'two': 'dos', 'three': 'tres', 'one': 'uno'}` and `tres`.
* The order of the key-value pairs would be random.
* We would not use index. We would use key to find the corresponding value. The key three maps to the value tres.
* The python dictionary is mutable.
>

<br/>

## Function works with dictionary

The `len()` function returns the number of key-value pairs.

The `in` function would search for the key. If the key exist in the dictionary, the function returns true. The dictionary uses a data structure called a hashtable to search the item. Therefore, no matter how many items are in the dictionary, the function would take same amount of time. Comparatively, the `in` function uses different algorithm for list. The time complexity depends on the length of list.

## word frequency

```python
def histogram(sentence):
    # We would create a dictionary and use it as counter.
    counter = dict()
    # We would use the for loop to traverse the string.
    for character in sentence:
        # The character has not been seen.
        if character not in counter:
            # The character has been seen for the first time.
            # The initial value would be 1.
            counter[character] = 1
        else:
            # The character has been seen for the next time.
            counter[character] += 1
    return counter


print(histogram("character"))

```

The output would be `{'c': 2, 'e': 1, 'r': 2, 'a': 2, 't': 1, 'h': 1}`.















































