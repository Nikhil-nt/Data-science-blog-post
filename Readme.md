## The Public 2019 Stack Overflow Developer Survey Results

### Motivation:
There are many competing views when it comes to breaking into a tech job , specifically when that job is aimed at the newest and hottest fields : artificial intelligence, data science, autonomous vehicles, or blockchain development, to name a few.

You may have heard statements like "you need to have a PhD to be a Data Scientist" or "you need a degree in Computer Science to become a Software Engineer."

Now, I have a personal viewpoint on the reality of these statements. You likely have your own viewpoint. But what does the data suggest? The future of what is required to move into developer roles is based on the ideas of those who are currently on the path to be leaders in the space. That is, current developers will determine the truth of these statements into the extended future.
Therefore, I used data from Stackoverflow’s 2019 Annual Developer Survey, to take a closer look at this question.

The survey data covers 88883 reviews from 213 countries and territories. The survey aims to understand multiple aspects of jobs related to software development and data analytics. There were more than 150 questions as a part of the survey, including:
"Do you program as a hobby or contribute to open source projects?"
"What are the work challenges you face?"

In this project i went through the following steps of Data Science process:
Business Understanding - Identify some questions 
Data Understanding - gather and understand the data based on the questions asked 
Data preparation- prepare the data for analysis 
Data modeling - Predict a response variable using machine learning model based on some feature variables.
Evaluate the results - Provide a conclusion.

### Installations:
* Numpy
* Pandas
* Matplotlib
* Sklearn
* Seaborn
* Python-3

### Description:

The enclosed data set is the full, cleaned results of the 2019 Stack Overflow Developer Survey. Free response submissions and personally identifying information have been removed from the results to protect the privacy of respondents. There are three files besides this README:

1. survey_results_public.csv - CSV file with main survey results, one respondent per row and one column per answer
2. survey_results_schema.csv - CSV file with survey schema, i.e., the questions that correspond to each column name
3. so_survey_2019.pdf - PDF file of survey instrument

The survey was fielded from January 23 to February 14, 2019. The median time spent on the survey for qualified responses was 23.3 minutes.

Respondents were recruited primarily through channels owned by Stack Overflow. The top 5 sources of respondents were onsite messaging, blog posts, email lists, Meta posts, banner ads, and social media posts. Since respondents were recruited in this way, highly engaged users on Stack Overflow were more likely to notice the links for the survey and click to begin it.

As an incentive, respondents who finished the survey could opt in to a "Census" badge if they completed the survey.

You can find the official published results here:

https://insights.stackoverflow.com/survey/2019

Find previous survey results here:

https://insights.stackoverflow.com/survey

### Summary:
Business Understanding- These were following businss questions i had:
* What are the employment status of non-technical graduates?
* What are the most popular languages?
* What determines the quality of life and the features involved in predicting the quality of life?

Data Understanding- 
To answer the questions i have to understand the data by collecting it and digging through the data.
I have also plotted the programmers from various countries where USA has the highest number of programmers.
The second plot was the number of graduates in this field. As usual computer science students were the highest.  

Question-1:  What are the employment status of non-technical graduates?
I have plotted a bar chart to see the employment status. Most of the graduates are employed full time,but the red column indicates that people drop out from the course and are not interested in working in that particular field. If we combine the red and green columns the rate of unemployment is high which shows that non technical grads find it difficult to get in to the tech field.

Question-2: What are the most popular languages?
Most of the programmers prefer to learn python followed html,css, javascript in the upcomming years making it the most popular language.

Question-3: What determines the quality of life and the features involved in predicting the quality of life?
* I have plotted a countplot to see the relationship between Hobby and Quality of life.
* The blue bar indicates those who don’t have a better life and the 0 on the x axis shows people who don’t program as a hobby.
This variable has a huge role in predicting the quality of life.
* I have created a list of variables i want to work with and used a label encoder to convert the strings to integer.
* I have dropped the null values.
* used onhotencoder to split the numerical categorial data into many columns.
* Ran the decision tree classification algorithm to use the categorial variables to predict the response.
* Finally i got a prediction score of 100.

Evaluate the results-
1. I plotted the employment status the non technical graduates and found that majority of them were employed but the number of unemployed graduates were more and have a tough time being employed in this field .

2. I saw the most python being the most demanding programming languages in future an aspirant should pursue.

3. Finally I predicted the quality of life based on various factors like Employment status, Hobby, student,workchallenge.

Legal:
This database - The Public 2019 Stack Overflow Developer Survey Results - is made available under the Open Database License (ODbL): http://opendatacommons.org/licenses/odbl/1.0/. Any rights in individual contents of the database are licensed under the Database Contents License: http://opendatacommons.org/licenses/dbcl/1.0/

TLDR: You are free to share, adapt, and create derivative works from The Public 2019 Stack Overflow Developer Survey Results as long as you attribute Stack Overflow, keep the database open (if you redistribute it), and continue to share-alike any adapted database under the ODbl.

Acknowledgment:

Massive, heartfelt thanks to all Stack Overflow contributors and lurking developers of the world who took part in the survey this year. We value your generous participation more than you know. <3
