# Spotify data analysis 
import pandas as pd
df=pd.read_csv('D:\spotify_top50_2021_vijaynandeshwar.csv')
print(df)

#HEAD
df.head(10)
df.head()

#type
df['artist_name'].dtype

#columns
df.dtypes

#axes
df.axes

#dimension
df.ndim

#shape and size
df.shape

df.size

#values 
df.values
#describe
df.describe()

#min and max
df.min()
df.max()

#mean,variance,sd
df.mean()
df.var()
df.std()

#drop
df.dropna()

#describe
df.describe()

#artist name
df['artist_name']

import numpy as np
y=np.arange(15).reshape(3,5)
print(y)

x=np.arange(15).reshape(3,5)
print(x)

o=[1,5,6,9]
b=[5,6,8,9]



# importing the required module
import matplotlib.pyplot as plt
#scatter plot
x = [1,2,3,4,5]

y = [2,4,6,8,10]

plt.scatter(x,y)

plt.show()

#line plot

x = [92,90,91,95,93]

y = [0.561,0.593,0.591,0.563,0.702]

plt.xlabel("x value")

plt.ylabel("Y value")

plt.title('Simple chart')

plt.plot(x,y)

#Bar Plot
artist_name= ['Dua lipa', 'Bruno mars', 'drake', 'Harry style', 'j balvin']

popularity = [92,90,85,94,99]

plt.bar(artist_name,popularity)

plt.show()

#pie chart
artist_name = 'Frogs', 'Hogs', 'Dogs', 'Logs'

popularity = [15, 30, 45, 10]

plt.pie(popularity, artist_name=artist_name, autopct='%1.1f%%')

# Equal aspect ratio

plt.axis('equal')

plt.show()


#
labels = 'Dua lipa', 'Bruno mars', 'drake', 'Harry style'

sizes = [15, 30, 45, 10]

plt.pie(sizes, labels=labels, autopct='%1.1f%%')

# Equal aspect ratio

plt.axis('equal')

plt.show()
