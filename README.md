# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

NAME: MADHU SHRUTHI A.R

REG: 212224050216
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
```
<img width="1219" height="224" alt="image" src="https://github.com/user-attachments/assets/b013126d-6f37-474e-8641-a94b893cd43e" />

```
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y)
plt.title('Line Plot')
```
<img width="726" height="589" alt="image" src="https://github.com/user-attachments/assets/b407cfab-d6e6-4b5a-9345-8ed9065c9cbb" />

```
x=[1,2,3,4,5]
y1=[3,5,2,6,1]
y2=[1,6,4,3,8]
y3=[5,2,7,1,4]
sns.lineplot(x=x,y=y1)
sns.lineplot(x=x,y=y2)
sns.lineplot(x=x,y=y3)
plt.title('Multi Line Plot')
```
<img width="691" height="589" alt="image" src="https://github.com/user-attachments/assets/1e125103-86a2-4952-96b2-aaa9238f0096" />

```
plt.figure(figsize=(8,5))
sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
plt.title("Fare Of Passenger By Embarked Town")
```
<img width="892" height="635" alt="image" src="https://github.com/user-attachments/assets/0724ba7c-b33d-461a-8be5-f26a2d691002" />

```
sns.scatterplot(x="Age", y="Fare", data=df)
plt.title('Scatterplot of Age vs Fare')
plt.show()
```
<img width="571" height="453" alt="image" src="https://github.com/user-attachments/assets/8c1b2b6c-55ae-4dc8-b3b2-6589919034ab" />

```
sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
plt.show()
```
<img width="571" height="453" alt="image" src="https://github.com/user-attachments/assets/5938f59e-9a0b-4685-87bf-c045c84fafdb" />

```
sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```
<img width="748" height="586" alt="image" src="https://github.com/user-attachments/assets/a14d3b8d-fc19-4488-8579-f2cd70f1a6ab" />

```
sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
plt.title("Age By Passenger Class")
```
<img width="750" height="606" alt="image" src="https://github.com/user-attachments/assets/58f69bc9-46e4-43f5-b2ec-d8c227627536" />

```
sns.violinplot(x="Pclass", y="Fare", data=df)
plt.title('Violin Plot of Fare by Passenger Class')
plt.show()
```
<img width="571" height="453" alt="image" src="https://github.com/user-attachments/assets/432fbb82-893d-4f0a-9672-399a5e870a8e" />

```
sns.kdeplot(data=df['Age'], fill=True)
plt.title('Density Plot of Passenger Ages')
plt.show()
```
<img width="585" height="453" alt="image" src="https://github.com/user-attachments/assets/03e1c1d4-9e86-426d-b205-2e618ca0a57f" />

```
numeric_df = df.select_dtypes(include=['float64', 'int64'])
corr_matrix = numeric_df.corr()
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
plt.title('Heatmap of Titanic Dataset')
plt.show()
```
<img width="597" height="503" alt="image" src="https://github.com/user-attachments/assets/68edd043-dffc-4a41-b8f4-e62fb46c01f1" />


# Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
