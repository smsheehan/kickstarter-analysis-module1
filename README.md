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
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90977689/134559406-56209a43-076c-488e-be03-b317aa12ef1b.png)

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
