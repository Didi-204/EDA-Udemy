# EDA-Udemy
an Azubi group assignment - an exploratory data analysis on udemy courses 
Contents
INTRODUCTION	2
1.1 Background	2
1.2 Objective	2
1.3 Understanding the Data	2
1.4 Hypotheses	3
1.5 Questions	3
EXPLORATORY DATA ANALYSIS	4
2.1 Data Cleaning	4
2.2 Data Analysis & Insights	4
FINDINGS	14
REFERENCES	14

INTRODUCTION

1.1 Background
University education is getting more and more expensive. The College Board indicates a 3% growth of tuition and fees for private and public colleges during the past two years. Online courses have become a great alternative to traditional education. The leading eLearning websites are Coursera and Udemy, which attract millions of users wanting to gain new skills. (Nechvolod, 2020)
Udemy is a massive online open course (MOOC) platform that offers both free and paid courses. Udemy, founded in May 2010, is an online learning platform aimed at professional adults and students. It allows people with varied expertise create a course and share content with others. Because of this, Udemy has hundreds of thousands of courses. Courses on Udemy cover nearly every subject and span every level – whether beginner, intermediate, expert etc. As of January 2020, the platform has more than 50 million students, 57,000 instructors teaching courses in over 65 languages and its website library contained over 150,000 courses. (Authors, 2020)

1.2 Objective
The goal of this project is to develop insights from the given dataset about the courses offered in four (4) subjects using tools and techniques of data science.


1.3 Understanding the Data
This dataset contains 3,682 records of courses from four(4) subjects (Business Finance, Graphic Design, Musical Instruments and Web Design) taken from Udemy. This dataset contains both free and paid courses. The level of difficulty of the courses are also varied. On the surface, there are 12 columns and 3,678 entries and 11,759,120 total number of subscribers. The column heads cover the following:
course_id - Course ID 
course_title - Course Title 
url - Course URL 
is_paid - Whether the course is free or paid 
price - Course Price 
num_subscribers - Number of subscribers 
num_reviews - Number of reviews 
num_lectures - Number of lectures 
level - Course difficulty 
content_duration - Duration of all course materials 
published_timestamp - Date that the course was published. 
Subject- Course subject 

 
1.4 Hypotheses
Below are a few points we would want to discover in our data analysis process:
1.	Count of the number of courses in each category 
2.	Count of the difficulty level of courses 
3.	Count of total number of subscribers as at 2017
4.	Courses with the most subscribers 
5.	Correlation between number of reviews and subscribers.
6.	Prices of courses
7.	Pattern of increment of courses from 2011 to 2017

1.5 Questions
These questions guided our analysis of the data
1.	Which subjects have the highest/least number of courses?
2.	What is the level of difficulty of the subjects?
3.	Which subjects/courses have the highest number of subscribers?
4.	What is the total number of subscribers as at 2017?
5.	Which free courses have the highest/least number of subscribers?
6.	Which of the subjects are expensive/cheap?
7.	What are the possible relationships that exist between the data provided?

EXPLORATORY DATA ANALYSIS
In analyzing this data set, we went through several processes including data cleaning, inspection, and the data analysis. We used Pandas to slice the data set, performed summary statistics using Numpy, and visualized the data using Matplotlib and Seaborn.

2.1 Data Cleaning
Data cleaning is a vital part of the data analysis process as it improves the quality of the data. A thorough look at our data revealed no null values or missing data. There was, however, a course, Mutual Funds for Investors in Retirement Accounts, with no lectures or subscribers, hence, we dropped it. This was done to ensure that the analysis was indeed a true representation of the data.

2.2 Data Analysis & Insights
Figure 2.1 – A BAR CHART SHOWING THE DISTRIBUTION OF COURSES BY THE SUBJECT
 

From the chart above, it can be observed that:
•	Web Development has the most courses (1,200), closely followed by Business Finance (1,195).
•	Musical Instruments and Graphic design are about halfway down with 680 and 603 courses respectively
Figure 2.2 - A BAR CHART SHOWING THE DISTRIBUTION OF COURSES BY THEIR LEVEL OF DIFFICULTY
 
From Figure 2.2 we realize that:
•	Most of the courses on Udemy (1,929) have content for all learning levels.
•	Material for beginners are the also quite high (1,270)
•	Intermediate (421 courses) and Expert level (58 courses) materials are quite low.
Figure 2.3 - A BAR CHART SHOWING THE DISTRIBUTION OF COURSES BY COST STATUS
 

A look at the Figure 2.3 above simply shows that most of the courses on Udemy are not free, as 91.6% of the total courses are paid.

Figure 2.4 – A CHART SHOWING THE TOP 10 MOST SUBSCRIBED COURSES
 
A look at the Figure 2.4 shows that;
•	Learn HTML5 Programming from Scratch is the most subscribed course on Udemy with 268923 subscribers.
•	Of the top 10 courses, only one (Free Beginner Electric Guitar Lessons) is not a Web Development Course.
•	Web development being the subject most subscribed to is reiterated.

Figure 2.5 - TOP 10 MOST SUBSCRIBED PAID COURSES
 
The chart (figure 2.5) above shows the top 10 paid courses that have the highest number of subscribers. 
•	The most subscribed paid course on Udemy is The Web Developer Bootcamp with 121,584 subscribers
•	Again, in this chart, there is only one course from a subject other than Web Development. Pianoforall - Incredible New Way To Learn Piano & Keyboard, the 5th most subscribed paid course (238,934 subscribers), is the only course from Musical Instruments or any other course aside Web Development.

Figure 2.6 – TOP 10 MOST SUBSCRIBED FREE COURSES
 In Figure 2.6 showing the most subscribed free courses we see that;
•	A Web Development course Learn HTML5 Programming From Scratch is at the top with 268,923 subscribers.
•	Eight out of the courses here are under the subject, Web Development.
•	In the top five, we have a Musical Instrument course, Free Beginner Electric Guitar Lessons, at 4th place with 101154 subscribers.
•	With 65,576 subscribers, Bitcoin or How I Learned to Stop Worrying and Love Crypto, a Business Finance course comes in 10th place.









Figure 2.7 TOP 10 MOST REVIEWED COURSES
 
From the chart above:
•	The Web Developer Bootcamp which is the most paid subscribed course is also the most reviewed course on Udemy with 27,445 reviews.
•	Two non-Web Development courses make it to this list, i.e Pianoforall - Incredible New Way To Learn Piano & Keyboard, Musical Instrument course which is the 10th most reviewed course with 7,676 reviews.

Figure 2.8 TOP 10 MOST REVIEWED PAID COURSES
 
This chart is nearly the same as Figure 2.7 (top 10 most reviewed) chart. Notable is
None of the courses cost less than 150

Figure 2.9 TOP 10 MOST REVIEWED FREE COURSES
 
We see from the chart (figure 2.9) above that
•	Of all the free courses, Learn HTML5 Programming From Scratch (which is also the most subscribed free course) has the highest number or reviews (8629)
•	Two Business Finance courses pop up here; Accounting in 60 Minutes - A Brief Introduction, the 7th most reviewed free course (4397 reviews) and Stock Market Investing for Beginners, the 9th most reviewed free course (2698 reviews).
•	All other courses are in this top ten charts are Web Development Courses.

Figure 3.0 – DISTRIBUTION OF FREE AND PAID COURSES BY SUBJECT
 
From the chart above, it can be observed that, 
•	In tangent with the distribution of courses and their respective subjects, Web Development has the most paid courses, followed by Business Finance, Musical Instruments and Graphic Design respectively.
•	On the contrary, however, there is shift when it comes to the free courses. Business Finance has more free courses than Web development, albeit marginal. Musical Instruments come in third with Graphic Design having the least number of free courses.

FIG 3.1 – DISTRIBUTION OF SUBJECTS BY THEIR LEVEL OF DIFFICULTY
 
In the chart (figure 3.1) above
•	Business finance is the subject with the highest number of expert level courses.
•	Business Finance has the most courses that suit all learning levels, followed by Web Development. Graphic Design comes next with just under 300 courses and Musical Instruments are not far off.
•	With the Intermediate level, Web Development has the most catering for this level, with Business Finance closely behind. The expert level follows this same distribution.
•	For beginner level courses, Web Development has the highest number of courses, followed by Business Finance, Musical Instruments and Graphic Design respectively.





Figure 3.2 – DISTRIBUTION OF NUMBER OF COURSES BY THE YEAR PUBLISHED
 
This chart allows us to observe that
•	There’s a trend running over the years. There’s a gradual increment in the number of courses in all subjects published from 2014 until 2016. In 2017, however, courses take a nosedive across subjects; quite heavily for Web Development and Graphic Design. 
•	In 2011, only a handful of courses were published on Udemy, and even then under only Web Development.












Figure 3.4 BOX PLOT OF THE PRICES OF SUBJECTS
 

From the above plot (figure 3.4);
•	Web development has the highest median price of 50 and the highest price of forty. About 50% of the prices of web development courses range from 20 to 115. From this we can say web development has the most expensive courses.
•	Even though Musical instruments has a median price of 40, an interquartile price range as 20 to 50 and some outliers, we can say it is cheaper relative to Graphic design since for the more than 25% of the courses range from 20 to 40.










Figure 3.5 MAP SHOWING CORRELATION BETWEEN PRICE, NUMBER OF SUBSCRIBERS, NUMBER OF REVIEWS, NUMBER OF LECTURES, CONTENT DURATION, PUBLISHED YEAR.
 

Figure 3.5 shows that:
•	There is a strong positive correlation between content duration and the number of lectures. We can infer that this is because more videos will obviously result in cumulatively longer durations of course content. 
•	Also, the number of reviews and number of subscribers have a strong positive correlation. This translates as the higher the number of users, the higher the number of reviews.


FINDINGS
•	The total number of subscribers as at 2017 was 11,759,120.
•	Since its launch in 2010, Udemy has seen a steady growth of course content and subscribers over the years from 2011 till 2016.

•	Per the dataset, Web Development is very popular among the subscribers of Udemy. This would explain why Web Development has the most courses; so, it can satisfy its large audience.

•	With a sample size of the top 10 most subscribed courses, there isn’t an inverse relationship between price and subscriptions. Of the top 10, four courses are paid for. Because over 90% of the total courses on Udemy are paid for, this is very encouraging.



REFERENCES
Authors, C. (2020, 08 06). Udemy. Retrieved from Wikipedia: https://en.wikipedia.org/wiki/Udemy
Nechvolod, A. (2020, April 27). How to build elearning websites like udemy or coursera. Retrieved from codica: https://www.codica.com/blog/how-to-build-elearning-website-like-udemy-or-coursera/



AN EXPLORATORY DATA ANALYSIS ON UDEMY by
Pascal Naa Zury
Phoebe Dadzie
Papa Nii Shang Annang
Prince Ani Acquah
