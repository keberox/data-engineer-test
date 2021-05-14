## Show the first 10 rows

```
import numpy as np
import pandas as pd
df = pd.read_csv('./cereal.csv')
print(df.head(5))
```
## Show all the columns
```
df.columns
```
## Does an increase in sugar lead to a higher rating?
```
sugar_df=df[['sugars','rating']]
print(sugar_df)
```


## Visualize 
```
import seaborn as sns
from matplotlib import pyplot as plt
hist = df.hist(figsize = (15,15))
```

## Insert into SQLite

```
import pandas as pd
import sqlite3

conn = sqlite3.connect('./data/catalog_sqlite.db')
cur = conn.cursor()


for chunk in pd.read_csv('./cereal.csv', chunksize=100, delimiter=','):
    chunk.to_sql(name='CEREAL', con=conn, if_exists='append', index=False)
    
```

## Show the top 10 cereals with the major combination of sugars and carbo.
```
SELECT
  name,
  SUM(carbo + sugars) AS total_carbs
FROM CEREAL
GROUP BY name
ORDER BY total_carbs DESC
LIMIT 10;
```

## Show the average of sodium among cereals with a rating higher than 38. 
```
SELECT
avg(sodium) as sodium_avg
FROM CEREAL
WHERE rating > 38
```


