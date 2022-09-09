## Find the most profitable company from the financial sector. Output the result along with the continent.

```
# Import your libraries
import pandas as pd

# Start writing code
profit_sorted = forbes_global_2010_2014[['company', 'continent', 'profits']].sort_values(by='profits', ascending=False)

profit_sorted[['company', 'continent']].head(1)
```
