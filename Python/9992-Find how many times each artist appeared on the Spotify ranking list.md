## Find how many times each artist appeared on the Spotify ranking list
Output the artist name along with the corresponding number of occurrences.
Order records by the number of occurrences in descending order.

```
# Import your libraries
import pandas as pd

# Start writing code
a = spotify_worldwide_daily_song_ranking

artist_count = a.groupby('artist')['trackname'].count().sort_values(ascending=False).reset_index()
```
