## workshop-Multivariate-analysis

# READING DATASET

import pandas as pd

import seaborn as sns

df=pd.read_excel('/content/FlightInformation.xlsx')

df.head()

df.dtypes

# NUMERICAL-CATEGORICAL

sns.scatterplot(y=df['Price'],x=df['Total_Stops'],data=df)

# CATEGORICAL-CATEGORICAL

sns.barplot(y=df['Price'],x=df['Source'],data=df)

# MULTIVARIATE ANALYSIS

df.corr()

sns.heatmap(df.corr(),annot=True)

# OUTPUT

![work1](https://user-images.githubusercontent.com/112301582/229767868-0dcfe210-e3b3-4b71-b9be-10d168e7a982.png)
![work 2](https://user-images.githubusercontent.com/112301582/229767910-cd108909-b8db-48a4-945d-3968ecc167bb.png)
![work3](https://user-images.githubusercontent.com/112301582/229767967-706828a5-14f0-4420-be0c-82b53d12b4b6.png)
![work4](https://user-images.githubusercontent.com/112301582/229767992-ab448584-7af2-4fcc-bb6b-0b8c70a13ce8.png)
![work5](https://user-images.githubusercontent.com/112301582/229768025-7dfff910-a2fa-4df5-b365-1febf50217f6.png)
