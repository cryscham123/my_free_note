## descriptive_statistics

### basic tools
```python
# Import the pandas library for data manipulation and analysis
import pandas as pd
# Import the numpy library for numerical operations
import numpy as np

shj = pd.read_csv('data/shj.csv', sep=',', encoding='utf-8')
shj

print(shj['HP'].describe())
```

### histogram
```python
import matplotlib
import matplotlib.pyplot as plt

%matplotlib inline
plt.hist(shj['HP'], alpha=0.4, bins=10, rwidth=1, color='blue')