# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
Line Plot <br>
```
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()
student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```
<img width="1115" height="662" alt="image" src="https://github.com/user-attachments/assets/d4e953bd-deff-4dec-afbe-cbeb039e4c5f" />
<img width="954" height="584" alt="image" src="https://github.com/user-attachments/assets/d8eb0001-48bc-4786-93d2-9053eb1ea5a6" /> <br>
Scatter Plot: <br> 
```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

<img width="1042" height="628" alt="image" src="https://github.com/user-attachments/assets/2439860f-efd8-4e69-82f9-054182dfe4c2" />
<img width="842" height="444" alt="image" src="https://github.com/user-attachments/assets/c8fc0adf-0ac5-468f-9d30-176adb151484" />
Pie Chart <br>
```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="1057" height="624" alt="image" src="https://github.com/user-attachments/assets/f32b17cf-a243-4417-8f4c-428bcc746931" />
<img width="1025" height="417" alt="image" src="https://github.com/user-attachments/assets/03ec1e8e-def9-4103-8913-f4bc173f282a" />
 Area Chart <br>
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="1063" height="586" alt="image" src="https://github.com/user-attachments/assets/b53992fe-a3f5-4aed-9336-4c68b4cfd8b1" />
 Bar Chart: <br>
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green']
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```
<img width="1048" height="602" alt="image" src="https://github.com/user-attachments/assets/d1900ff9-6b5d-45b2-9b49-8ad6f03248b0" />
 Histogram <br>
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='black', alpha=0.5)
plt.show()
```
<img width="1047" height="471" alt="image" src="https://github.com/user-attachments/assets/b5337bda-6c02-4f1d-859a-f07938693557" />
 Box Plot: <br>
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
<img width="1101" height="434" alt="image" src="https://github.com/user-attachments/assets/e0d3d15c-24b2-425a-be88-699c5e2a9124" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
<img width="1119" height="600" alt="image" src="https://github.com/user-attachments/assets/5b59f1fd-47a1-4489-a85a-9e34d8219303" />

# Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
