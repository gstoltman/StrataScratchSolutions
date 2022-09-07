## Find songs that have ranked in the top position. Output the track name and the number of times it ranked at the top. Sort your records by the number of times the song was in the top position in descending order.

```
# Import your libraries
import pandas as pd

df = spotify_worldwide_daily_song_ranking

top_rank = df[df['position'] == 1]

top_rank.groupby('trackname')['position'].sum().sort_values(ascending=False).reset_index()
```
