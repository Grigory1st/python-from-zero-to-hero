# Week 4: Debugging Common Issues

### IndexError
Accessing out of range.

```python
lst = [1,2]
print(lst[2])  # IndexError

# Fix: Check len
```

### KeyError
Invalid dict key.

```python
d = {"a":1}
print(d["b"])  # KeyError

# Fix: Use get()
print(d.get("b", "Not found"))
```

### TypeError with Sets
Sets don't support indexing.