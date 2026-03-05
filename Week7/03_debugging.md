# Week 7: Debugging Common Issues

### Broad Except
Catching all exceptions hides bugs.

```python
try:
    # code
except:  # Bad
    pass
```

### Not Raising Appropriate Exceptions
Use built-in or custom.

### Finally Not Used for Cleanup
Use finally for resources.