# Statistical Analysis
```python
import seaborn as sns
import matplotlib.pyplot as plt

def plot_feature_importance(df):
    plt.figure(figsize=(10, 6))
    sns.heatmap(df.corr(), annot=True, cmap='coolwarm')
    plt.show()
```