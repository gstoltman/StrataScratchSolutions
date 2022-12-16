## Find all Lyft drivers who earn either equal to or less than 30k USD or equal to or more than 70k USD.
Output all details related to retrieved records.

```
# Import your libraries
import pandas as pd

# Start writing code
lyft_salary = lyft_drivers[(lyft_drivers['yearly_salary'] <= 30000) |
                           (lyft_drivers['yearly_salary'] >= 70000)]
```
import sys

n = int(input().strip())

for _ in range(n):
    n = int(input().strip()) - 1
    threes = 3 * (n // 3) * (((n // 3) + 1) / 2)
    fives = 5 * (n // 5) * (((n // 5) + 1) / 2)
    fifteens = 15 * (n // 15) * (((n // 15) + 1) / 2)
    final = threes + fives - fifteens
    
    print(int(final))
```
