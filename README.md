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
# Line Graph
```
import matplotlib.pyplot as plt
x= [0,1,2,3,4,5]
y=[0,1,4,9,16,25]
plt.plot(x,y)
plt.show()
```

<img width="836" height="582" alt="image" src="https://github.com/user-attachments/assets/9ce3e206-197d-41a7-bc8a-5915f0f80f10" />

```
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,4,1]
plt.plot(x1, y1, label="line 1")

x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x2, y2, label="line 2")

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Two lines on same graph!')

plt.legend()
plt.show()
```

<img width="713" height="575" alt="image" src="https://github.com/user-attachments/assets/597c797d-3e72-400c-8c65-583203c1079b" />


```
import matplotlib.pyplot as plt

x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]

plt.plot(x, y, color='red', linestyle='dashed', linewidth = 5, marker='o', markerfacecolor='blue', markersize=14)

plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Line customization!')

plt.show()
```

<img width="695" height="566" alt="image" src="https://github.com/user-attachments/assets/3997bbb5-a114-40e7-9f06-ee9bcaf1401f" />

# Scatter Plot
```
import numpy as np
x = np.arange(0,10)
y = np.arange(11,21)
x
y
```

<img width="372" height="51" alt="image" src="https://github.com/user-attachments/assets/7e876df7-b5a8-4fe4-a90f-bd262f537bff" />

```
y=x*x
y
```

<img width="473" height="44" alt="image" src="https://github.com/user-attachments/assets/d3c4782f-867c-4125-82db-93980688b0d4" />

```
plt.plot(x, y, 'g*', linestyle='dashed', linewidth = 2, markersize = 14)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('2d Diagram')
```

<img width="707" height="599" alt="image" src="https://github.com/user-attachments/assets/7de06b24-1679-4b5c-bcdf-d2b49186b45a" />

```
np.pi
```

<img width="195" height="40" alt="image" src="https://github.com/user-attachments/assets/0a8f35b5-15b5-4918-850f-0756a3448a41" />


```
x = np.arange(0, 2*np.pi, 0.1)
y = np.sin(x)
plt.title("sine wave form")

plt.plot(x,y, 'go', markersize=8, color="pink")
plt.show()
```

<img width="725" height="596" alt="image" src="https://github.com/user-attachments/assets/d05512de-988f-436e-8019-9700bfea09c2" />

# Area Chart
```
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

<img width="697" height="517" alt="image" src="https://github.com/user-attachments/assets/85b2b558-9e7a-43cf-8f73-417f3c4451b9" />


# Bar Chart
```
import matplotlib.pyplot as plt
val=[5,6,3,7,2]
n=["A", "B", "C", "D", "E"]
plt.bar(n,val,color="green")
plt.show()
```

<img width="701" height="516" alt="image" src="https://github.com/user-attachments/assets/2913d73f-fd67-4d64-9c1b-d148286f8bf2" />


```
import matplotlib.pyplot as plt 
val=[5,6,3,7,2] 
n=["A", "B", "C", "D", "E"] 
plt.barh(n,val,color="green")
plt.show()
```

<img width="674" height="519" alt="image" src="https://github.com/user-attachments/assets/ddfa2db0-7675-4272-9fce-c07a9009b810" />

```
import matplotlib.pyplot as plt
height=[10,20,30,40,50]
names=["one", "two", "three", "four", "five"]
c1=["red", "green"]
c2=["b","g"]
plt.bar(names,height, width=0.8,color=c1)
plt.xlabel('x axis')
plt.ylabel('y axis')
plt.title("Bar Chart")
plt.show()
```

<img width="737" height="582" alt="image" src="https://github.com/user-attachments/assets/0cd42cdd-7480-4911-8989-d74562a95d9e" />

# Histogram
```
import matplotlib.pyplot as plt
age=[2,5,70,30,45,50,45,43,40,44,60,7,13,57,18,90, 77, 32, 21, 20,40]
range=(0,100)
bins=10
plt.hist(age,bins, range, color="green", histtype='bar', rwidth=0.8)
plt.xlabel('Age')
plt.ylabel('No of People')
plt.title("Histogram")
plt.show()
```

<img width="735" height="577" alt="image" src="https://github.com/user-attachments/assets/2d78058c-3094-4780-a5a7-57b9088d6e75" />

```
import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] 
plt.hist(x,bins=10,color='blue', alpha=0.5)
plt.show()
```

<img width="666" height="522" alt="image" src="https://github.com/user-attachments/assets/4e0326b1-7f68-4f98-93db-1bc54ae9bc13" />

# Box Plot
```
import matplotlib.pyplot as plt 
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

<img width="702" height="441" alt="image" src="https://github.com/user-attachments/assets/d57827b3-ca51-4eb4-8977-a5376d0a7c9e" />

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="704" height="600" alt="image" src="https://github.com/user-attachments/assets/df47a8dc-034c-4d2e-9d26-058dcfca5f54" />

# Pie Chart
```
import matplotlib.pyplot as plt
activities=["eat", "sleep", "work", "play"]
slices=[3,7,8,6]
colors=['r','y','g', 'b']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1, 0), radius=1.2, autopct='%1.1f%%')
plt.legend()
plt.show()
```

<img width="544" height="498" alt="image" src="https://github.com/user-attachments/assets/fc506d2b-9e14-4d90-9129-20e393f3a559" />





# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
