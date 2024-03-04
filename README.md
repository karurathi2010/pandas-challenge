# pandas-challenge
# PyCity Schools Analysis

Two data sets were provided for the analysis
1)	School_complete
2)	Student_complete
To get a clear picture, both data sets are combined into a single data frame and created the following Dataframes for further studies.

## District Summary:
This gives an overall understanding of the schools at the district level like

•	Total number of students 
•	Total number of unique schools
•	Total budget 
•	Average marks in reading and math
•	Overall passing percentage

## School Summary:
From here onwards we are considering the factors affecting the passing percentage of the students at the school level. For that set the index as “School name”.
Then found the following parameters based on the school name and combined those series into a sinas  dataframe as ‘Per_school_summary’.

•	School Type	
•	Total Students	
•	Total School Budget	
•	Per Student Budget	
•	Average Math Score (students per school with reading scores of 70 or higher)
•	Average Reading Score (students per school with reading scores of 70 or higher)
•	% Passing Math	
•	% Passing Reading	
•	% Overall Passing

## Highest-Performing Schools (by % Overall Passing):
Using the  ‘Per_school_summary’ Dataframe understand the highest performing schools by simply sorting the the data '% Overall Passing' col## umn in descending order.

## Bottom Performing Schools (By % Overall Passing):
Using the  ‘Per_school_summary’ Dataframe understand the highest performing schools by simply sorting the the data '% Overall Passing'##  column in ascending order.

## Math Scores by Grade:
Here we are considering the grade-level average math scores of each school to understand whether the grades have any ## influence on the passing rate.

## Reading Score by Grade:
The same procedure in Math Scores by Grade is##  repeated here on reading scores.

## Scores by School Spending:
The idea behind this step is to understand whether the budget spending per student at each school has any influence on the overall passing rate. For that created ‘Bins’ on "Per Student Budget" and added a new column to the data frame as “Spending Ranges (Per Student)”.
The above  data frame is  ‘grouped by’ Spending Ranges (Per Student)” and created a summarized data frame with the following columns, 

•	Average Math Score	
•	Average Reading Score	
•   % Passing Math	
•	% Passing Reading	
•	% Overall Passing
 Which gives a better understanding of the relationship between budget spending and overall passing rate. 

## Scores by School Size:
Here we are considering the school size and passing rate. So the same logic applied in the above case is used here as well.
Here created ‘Bins’ on  "Total Students" and added a new column to the data frame as “School Size” and then  ‘grouped by’  “School Size” and created a summarized data frame with the same columns as above. 
Which gives a better understanding of the relationship b## etween school size  and overall passing rate. 

## Scores by School Type:
Here using the “per_school_summary “ data frame performs the groupby function on “school type” and creates a summarized data frame with the following columns.

•	Average Math Score	
•	Average Reading Score	
•   % Passing Math	
•	% Passing Reading	
•	% Overall Passing
Which gives a better understanding of the relationship between school type  and overall passing rate. 

## Conclusions:
There are several interrelated factors affecting the overall passing rate of schools.
Considering the above analysis there two factors are directly related to the passing rate.

1)	School Type:
In the provided data set we had two types of schools “ District” and “Charter”.
From the “Scores by School Type” data frame, it is very clear that the “Charter” school has the highest passing rate.

2)	School Size:
Also considering the “Scores by School Size” data frame we can say that the schools hav
ing a small size (Small (<1000) ) have the highest passing rate.

One interesting thing is that compared to district schools charter schools are small in size. So it is very clear that the factors are inter related.
