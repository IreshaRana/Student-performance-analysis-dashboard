# Student-performance-analysis
## Background
As a vonluntary project, I conducted a student performance analysis for a course I was teaching. I was able to uncover insights and provide data-driven recommendations to improve student peroformance. 

Requirements for such an analysis:
- This course was suffering from low grades. There was a need to increase grades, so that the course would become more popular among students. 
- As this course was being taken by students from various degree programs, the course coodinator wanted to analyse for any areas of support required. 

As the original project cannot be shared owing to confidentiality, I tried to replicate it.

## Project goal, objectives and deliverables  
Goal: 
- To identify areas of improvement to increase course grades.
 
Objectives:
- Analyze patterns in student performance, online engagement and enrolement data.
- Identify factors influencing success or underperformance.
- Visualize insights to share with stakeholders (course coordinator, degree program leads).
- Provide recommendations to improve teaching and learning activities.

Deliverables:
- Key statistics and insights about the student performance.

## Data 
I generated a synthetic data set for this project, as the original data is confidential.
Student performance data:
1.	Student ID: Unique identifier for each student (e.g., S001, S002, ..., S480).
2.	Program Code: values from 1 to 15 (representing different programs).
3.	Assessment scores: Scores for the assessments, calculated as per the weights (15% for the quiz, 35% for the written assessment, 35% for the group project, and 15% for the reflective piece).
4.	Final Score: Weighted average of the assessments
Online engagement (with the university Learning Management System or the LMS) data:
5. Log-in Frequency: number of times per week
6. Session Duration: time spent on LMS per week
Enrolment data:
8.	Enrollment Status: Full-time or Part-time

## Data preparation
In the original project, 
- I had to merge data files.
  - I retrieved student performace data, student engagement data and enrolment data from 3 different sources and merged them together.
  - There were data mismatches between the datasets, so only the students who had a live enrolment status (fulltime or parttime) were included in the final analysis.
- I conducted some data manipulations.
-   The log-in frequency and session durations data were in a log fie. I manilupated the data so that I could get an average per week value for the duration of the semester.
  
For this project, 
- A synthetic dataset was generated. 

## Data generation and Analysis
- Generate data
  - Generated a synthetic data  to closely resemble the original merged dataset in terms of variables and student numbers (~480).  
- Explore data
  - Calculate summary statistics
- Data manipulation
  - Adding a grades column
- Analysis
  - Assessment scores distribution (visualisation:box-plot)
  - Program code over grades (visualisation:bar chart)
  - Enrolment status over grades (visualisation: pie charts)
  - Session duration over final scores (visualisation: scatter plot)

Code: Open the Jupyter notebook - [Student performance.ipynb](Student performance.ipynb)
Technologies used: R programming (dplyr, tidyr, ggplot)

## Conclusions and Recommendations
In the original project (with the real dataset), I came up with the following insights from the analysis
- Assessment scores for 3B were generally lower when compared to other assessments, with a lower average score and lower range.
- Students from certain degree programs were having higher failure %s.
- Session duration were seen to have a somewhat positive relationship with the final scores, that is, when session duration is high, the students were having higher grades.
- There was no considerable change in grades when full time and part time students were compared.

Recommendations:
- Provide clearer guildelines for Assessment 3B and revisit rubric criteria.
- Have a discussion with program leads of low performing degree programs to see how this course aligns with their overall leaning objectives.
- Encourage students to actively engage in course material via reminders and increasing inteactive elements in the LMS to further encourage engagement. 

 
## Next steps
- Analyse student enagement throughout the semster, so that timely action can be taken to increase engagement (and thereby their final scores).
- Set metrices for next course offering and monitor the progress. (e.g. engagement metrices for first quarter, first half etc.)

  


