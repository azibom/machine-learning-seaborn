# machine-learning-seaborn
how can you use seaborn in python

#### Seaborn is a library for making statistical infographics in Python. It is built on top of matplotlib and also supports numpy and
#### pandas data structures. It also supports statistical units from SciPy.

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sb
import pandas as pd
data = pd.read_csv('c://data.csv')
```
#### you should test all of this charts by yourself to understand them

## Strip Plot
```python
# plots the distribution of variables for each category as individual datapoints
sb.stripplot(x='A', y='B', data=data, size=10)
plt.show()

# or

# This function is similar to stripplot(), but the points are adjusted (only along the categorical axis)
# so that they don’t overlap
sb.swarmplot(x='A', y='B', data=data)
plt.show()
```

## Box Plot
```python
sb.boxplot(x='A', y='B', data=data)
plt.show()
```

## Joint Plot
#### visualize a bivariate distribution
```python
sb.jointplot(x='A', y='B', data=data, kind='scatter')
plt.show()
```

## Pair Plot
```python
sb.pairplot(smartphones, hue='Name')
plt.show()
```

I hope this data will be useful to you.


