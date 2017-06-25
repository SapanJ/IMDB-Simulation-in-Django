# IMDB-Simulation-in-Django
Django based web solution for rating and reviewing Movies.

Problem Statement
The objective of this assignment is to build a movie review website similar to IMDB
Solution:
I have tried to cover my high level understanding about Django by using below given points.
1.	Database Design
2.	Touch Points
3.	Focus Areas
4.	Functional flow
5.	Software Used

Database Design
Table 1: MovieData
Movie_ID	Movie_Name	Director_Name	Genre	Release_Year
<PK>	Char 	Char	Char	Year/Int

Table 2: ReviewData
ID	Movie_ID	Rating	Review(NULL=True)
<PK>	<FK>	Int	Text

Touch Points
From Django point, below things are considered while designing the solution
•	Customized URL
•	Utilization of Templates
•	Django Admin site and super user access
•	Filters and Tags for easiness
•	Normalized Data Base
Focus Areas
•	Exception Handling. Example: HTTP404
•	ORM
Functional Flow
Just calling the URL will take you to the index.html, you will get dynamically fetched list of all Movies where each movie name is a <link> that will call another page with customized URL for the average rating and number of reviews given to that movie. Generally reviewer won’t write comment every time, so I am calculation how many users have actually wrote something as a review, so we can use it for sentiments analysis. Current DB does not carry user/reviewer information but we can add it easily.
Below attached pictures brief you about the functional structure of the solution. 
    
Data Base design Pictures from Admin site.
 

   
 
Software Used
Eclipse IDE with pydev environment
Python Version: 2.7.12
Django Version: 1.11.2
