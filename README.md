
## World Cup Data Engineering Project

### Aim of the project
The aim of this project is to explore the possibility of the interaction between postgresql and python
### Description of the used data
The data used in this project eas obtained from [Kaggle](https://www.kaggle.com/datasets/rajkumarpandey02/fifa-world-cup-attendance-19302022?select=FIFA+World+Cup+Award.csv). And it is made of three CSV files. the file containing data related to world cup attendance from 1930 up to 2022. Here we are going to describe each file with pictures showing its respective columns individually\
1. Attendance: having general information related to each world cup(Host country, total attendance, etc..
![image](https://user-images.githubusercontent.com/120035660/229309079-42ffb04c-f3cc-4638-8f54-f74c483f758e.png)

2. Awards: containing information for every and each spefic awards winners at each world cup
![image](https://user-images.githubusercontent.com/120035660/229309134-12641c27-df4a-4953-8b11-53fc5ef29f0f.png)

3. Finals: contains each and every finall information(winner, score, etc
![image](https://user-images.githubusercontent.com/120035660/229309177-3611deb4-9762-4559-ba6c-12ad3be5e0d8.png)



### General Project Overview
#### Used libraries
The main python library used in this case is [psycopg2](https://www.psycopg.org/docs/), which is the most popular PostgreSQL database adapter for the Python programming language. 
We will also be using [pandas](https://pandas.pydata.org/docs/), will be usefull as some of its functions and methods will be needed for this project.
#### Project overview
##### Getting the dataset from Kaggle
The first task consists of geting or downloading the three csv files forming our dataset from Kaggle, and for this project we included them in our working directory
##### Creating the database in postgresql with the tables 
Here we used the famous python library called psycopg2, which allows us to interect with our postgresql in python. So for this a database called worldcup was created with three tables called attendance, awards and finals. And all was achieved after ensuring a coonection to our database was available
##### Inserting values in the thre different tables
Here we inserted all values present in our csv files into the three tables created in postgresql.(At this stage we faced a problem related to the last table or the table called "final", but fortunatelly we just noticed that it wa a simple syntax error:))))))
\
All the detailed code and explanation can be found [here](https://github.com/JulienAganze/World-Cup-Data-Engineering-Project-Postgres/blob/master/Data_Engineer_Project1.ipynb)
