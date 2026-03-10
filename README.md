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
import matplotlib.pyplot as plt

%matplotlib inline
```
```
import numpy as np
```
```
x=np.arange(0,10)
y=np.arange(11,21)
```
```
a=np.arange(40,50)
b=np.arange(50,60)
```
```
plt.scatter(x,y,c='g')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
<img width="775" height="600" alt="Screenshot 2026-03-10 101958" src="https://github.com/user-attachments/assets/7d4367f4-a11a-4bc8-846b-79f1923d0c1e" />

```
y=x*x
```
```
plt.plot(x,y,'r*',linestyle='dashed',linewidth=2, markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.show()
```
<img width="733" height="594" alt="Screenshot 2026-03-10 102018" src="https://github.com/user-attachments/assets/859ac3e8-36df-4a46-9c04-da020310310b" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
plt.show()
```
<img width="733" height="514" alt="Screenshot 2026-03-10 102029" src="https://github.com/user-attachments/assets/8b17f84f-fd2d-41a3-a262-eb19068217c7" />

```
x = np.arange(1,11) 
y = 3 * x + 5 
plt.title("Matplotlib demo") 
plt.xlabel("x axis caption") 
plt.ylabel("y axis caption") 
plt.plot(x,y) 
plt.show()
```
<img width="773" height="592" alt="Screenshot 2026-03-10 102036" src="https://github.com/user-attachments/assets/8a5df340-c606-4045-bc86-bf5e843df1c7" />

```
np.pi
```
<img width="198" height="64" alt="Screenshot 2026-03-10 102452" src="https://github.com/user-attachments/assets/5de92e33-61c3-42ca-aa2c-911e8fce9e1d" />

```
# Compute the x and y coordinates for points on a sine curve 
x = np.arange(0, 4 * np.pi, 0.1) 
y = np.sin(x) 
plt.title("sine wave form") 

# Plot the points using matplotlib 
plt.plot(x, y) 
plt.show()
```
<img width="812" height="569" alt="Screenshot 2026-03-10 102045" src="https://github.com/user-attachments/assets/2c1036d2-e1d8-4348-9e82-35a627d3301f" />

```
#Subplot()
# Compute the x and y coordinates for points on sine and cosine curves 
x = np.arange(0, 5 * np.pi, 0.1) 
y_sin = np.sin(x) 
y_cos = np.cos(x)  
   
# Set up a subplot grid that has height 2 and width 1, 
# and set the first such subplot as active. 
plt.subplot(2, 1, 1)
   
# Make the first plot 
plt.plot(x, y_sin,'r--') 
plt.title('Sine')  
   
# Set the second subplot as active, and make the second plot. 
plt.subplot(2, 1, 2) 
plt.plot(x, y_cos,'g--') 
plt.title('Cosine')  
   
# Show the figure. 
plt.show()
```
<img width="761" height="575" alt="Screenshot 2026-03-10 102051" src="https://github.com/user-attachments/assets/c98314e9-e12e-4c01-89ed-06003038faa8" />

```
## Bar plot

x = [2,8,10] 
y = [11,16,9]  

x2 = [3,9,11] 
y2 = [6,15,7] 
plt.bar(x, y) 
plt.bar(x2, y2, color = 'g') 
plt.title('Bar graph') 
plt.ylabel('Y axis') 
plt.xlabel('X axis')  

plt.show()
```
<img width="794" height="590" alt="Screenshot 2026-03-10 102057" src="https://github.com/user-attachments/assets/1000bfdb-d04e-42bd-a7aa-a2b4ae62da16" />

```
a = np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27]) 
plt.hist(a) 
plt.title("histogram") 
plt.show()
```
<img width="736" height="539" alt="Screenshot 2026-03-10 102104" src="https://github.com/user-attachments/assets/14f6bb3a-b75c-4a87-9f81-c0290a53c05d" />

```
data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=False);  
plt.show()
```
<img width="743" height="565" alt="Screenshot 2026-03-10 102109" src="https://github.com/user-attachments/assets/e520ad15-ec3e-496c-8b9c-a888dc83aae3" />

```
data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=True);
plt.show()
```
<img width="759" height="524" alt="Screenshot 2026-03-10 102117" src="https://github.com/user-attachments/assets/c42ea2bb-505b-4293-a06f-d0964121a9a5" />

```
data
```
<img width="800" height="752" alt="Screenshot 2026-03-10 102127" src="https://github.com/user-attachments/assets/ff7516ff-8e90-40a0-92a9-39c8ea4383ff" />

```
# Data to plot
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0.4, 0, 0, 0)  # explode 1st slice

# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors,
autopct='%1.1f%%', shadow=False)

plt.axis('equal')
plt.show()
```
<img width="816" height="577" alt="Screenshot 2026-03-10 102135" src="https://github.com/user-attachments/assets/0f0c2361-6d24-4028-a6bf-d674dc5ae968" />



# Result:

Thus Data Visualisation using matplotlib library has been done and verified.
