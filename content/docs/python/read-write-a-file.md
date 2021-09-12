---
title: Read/Write a File Python
type: docs
---

# `Python` : Read/Write a File

## Read an entire file
```python
with open("file.txt") as f:
    content = f.read()
```
## Read a file line by line
```python
with open("file.txt") as f:
    for line in f.readlines():
        # Do something with each line
```

## Write to a file
```python
with open("file.txt", "w") as f:
    f.write("Something")
```

## Append to a file
```python
with open("file.txt", "a") as f:
    f.write("Something!")
```
