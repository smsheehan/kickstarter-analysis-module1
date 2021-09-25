# Kickstarting with Excel

## Overview of Project
Kickstarter is a crowdfunding platform that enables entrepreneurs to attract funding to help bring a project or product from idea to implementation.  According to wikipedia, https://en.wikipedia.org/wiki/Kickstarter, since July 2021 there have been approximately 205,00 successfully funded projects which makes this an interesting data set for learning data analytics skills.  This was a project to evaluate a kickstarter data set to try to understand factors that play a role in a kickstarter's success or failure.  Specifically, much of the focus of this project was in the category of theater and subcategory plays.

### Purpose
The purpose of the project was to test whether we could implement concepts learned in the module lessons to provide two different analyses.  The purpose of the analyses was to see if we could glean useful information from analyzing previous kickstarter outcomes based on launch date and from analyzing previous kickstarter outcomes based on the initial dollar goals of those projects.  This was done under the auspices of helping our fictional friend, Louise, understand if these two variables (launch date, funding goal) impacted the success of projects on kickstarter. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
This analysis starts with the need to take our "Date Created Conversion" column in which we had previously converted date from unix format, and extract out just the year.  The function used to do this was straightforward.  INSERT LINK TO FUNCTION.   I then created a pivot table and applied appropriate filters and sorting to achieve the following table
https://github.com/smsheehan/kickstarter-analysis-module1/blob/main/Screenshot%20theater%20outcomes%20by%20launch%20date%20pivot%20table.png
After ensuring the table was correctly displayed, I used the Insert tab in excel to create a line chart, which looked like this:
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90977689/134559226-8e574f1b-e845-4e7d-ae7a-d84b7fc1c93e.png)

### Analysis of Outcomes Based on Goals
This analysis required the creation of 8 columns (Goals, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled) in a new sheet and I needed to create functions extract the relevant information for the subcategory "plays" from the main kickstarter data worksheet.  For the Number Successful/Failed/Canceled columns, this was accomplished using the countifs function.  Here is a representative function for the Number Successful column:  INSERT LINK TO FUNCTION HERE.  The remaining columns required only simple math functions to calculate the sum and percentage where appropriate.  I then inserted a line chart which looked like this:
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90977689/134559406-56209a43-076c-488e-be03-b317aa12ef1b.png)

### Challenges and Difficulties Encountered
The biggest challenge associate with this assignment was getting comfortable with writing functions that pull data from a different worksheet.  Having never done this before, it took some time for me to get used to the fact that the function input line from the page you are typing in persists when you click into a different worksheet to select cells.  The other challenge was that it took me some time to understand how to copy and paste functions from one cell to another without disrupting the original function.  Specifically I realized that once I have copied a formula, I need to "unhighlight" the original formula before clicking into another cell, otherwise the original formula will be replaced with the name of the cell that I was clicking into.  This makes sense based on the functionality that allows us to build our functions by clicking into cells, but took some time for me to get used to this.  The biggest difficulty I ran into was making sure the column formatting was appropriate.  For example, when extracting the year from the "Date Created Conversion" column, my output wasn't displaying properly because I kept trying to format the column as a date.  It took me a while to realize that the proper column format needed to be  "general" in order to correctly display the year.  Additionally , in creating percentages, I multiplied by 100 to create the percentage withing the function.  However, when I first created my line chart I noticed the Y axis didn't display the percentage symbol which would make the chart confusing to the reader.  I then realized I needed to remove the times 100 from my function and format the receiving column as percentage.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
