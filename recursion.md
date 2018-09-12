### 1. use recursion to get complete set
example nset = [1, 2, 3]
```
def get_complete_set(n=[1, 2, 3]):
    result = [[]]
    for item in n:
        result += [res + [item] for res in result]
    return result
```