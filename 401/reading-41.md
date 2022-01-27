# Python Iterators

for-in loops are very elegant and readable
- iterator protocol allows us to implement it in our own custom classes

## Python Iterators That Iterate Forever

```python
repeater = Repeater('Hello')
for item in repeater:
    print(item)
```

Creating a Repeater class to repeatedly return a single value

```python
class Repeater:
    def __init__(self,value):
        self.value = value

    def __iter__(self):
        return RepeaterIterator(self)
```

RepeaterIterator is a helper class to get for-in iteration to work

```python
class RepeaterIterator:
    def __init__(self, source):
        self.source = source

    def __next__(self):
        return self.source.value
```

- __init__ method links the RepeaterIterator to the source object
- __next__ method reaches back into the source and returns the value associated with
