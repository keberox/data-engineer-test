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


