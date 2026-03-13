# ETL with Pandas
```python
import pandas as pd

def clean_and_transform(raw_csv):
    df = pd.read_csv(raw_csv)
    df.dropna(inplace=True)
    df['normalized_score'] = (df['score'] - df['score'].mean()) / df['score'].std()
    return df
```