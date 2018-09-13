### 1. Get degree of a non-negative integer array
Degree equals the maximum counts of repeated word
```
from collections impor defaultdict

def get_array_degree(nums=[1, 1, 2, 2, 2]):
    pos = defaultdict(list)
    for i, num in enumerate(nums):
        pos[num].append(i)
    degree = max(map(len, pos.values()))
    return degree

```
