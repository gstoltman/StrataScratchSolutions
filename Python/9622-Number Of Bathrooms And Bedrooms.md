## Find the average number of bathrooms and bedrooms for each city’s property types. Output the result along with the city name and the property type.

```
# Import your libraries
import pandas as pd

# Start writing code
airbnb_search_details.groupby(['city', 'property_type'])[['bathrooms', 'bedrooms']].mean().reset_index()
```
