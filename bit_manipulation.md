### 1. how to know a integer is a 2 power number
Python Code:
```
# retrun True if it is
def is_2power_integer(n):
    if n <= 0:
        return False
    return n & (n - 1) == 0
```