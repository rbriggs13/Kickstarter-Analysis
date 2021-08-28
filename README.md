# Kickstarting Analysis

## Project Overview

### Purpose
  The purpose of this project was to aid Louise in launching her play called _Fever_. This assistance could be provided by analyzing the data from past kickstarter projects that were in the theater category. The outcomes of these projects could then be compared to both the launch dates and monetary goals of the various campaigns in order to determine a reasonable amount of money to ask for and when best to launch the kickstarter. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
  This analysis was performed by first using a pivot table to sort our the data irrelevant for this particular analysis. What was left in the table were the months any theater projects begain and the amount of successful, failed, or canceled theater projects for those particular months. The following graph was created from the resulting table.
  ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/87343629/131198626-bc753cf8-eb34-430d-97dd-8252f3913966.png)
  
### Analysis of Outcomes Based on Goals
  This analysis was performed by first determining various goal categories, such as $1,000 to $4,999 for example. Then the amount of successful, failed, and canceled campaigns were obtained for each category. Finally that data was used to determine the percentage of projects were successful, failed, or were canceled for each goal range. The resulting percentages were then used to create the following graph.
  ![Outcomes_vs_Goals](https://user-images.githubusercontent.com/87343629/131199071-da493d16-803a-4a53-b7e7-96efd448577d.png)

### Challenges and Difficulties Encountered
  The largest challenges faced across both analyses had to do with an error with a formula during the Goal based analysis. I specifically encountered a lot of issues with the COUNTIFS formula for calculating the number of successful, failed, and canceled projects. However most of these challenges were not based on misunderstanding the formula but based on typos made while filling it in. For example I had used "play" to refer to the subcategory to search for rather than "plays" This resulting in 0 results for everything, which was incorrect. Once I corrected this error, most of the data came through correctly except for the last goal range, which was greater than 50,000. In the COUNTIFS formula for that I had accidently typed a "<" rather than a ">" resulting in very incorrect data. However this mistake was found and corrected. 
## Results
  The first conclusion that can be drawn from the launch date analysis is that May is the best month to launch a theater kickstarter. While there is also a increase in failures the difference between the number of successful projects compared to the ones that failed is the largest in this month. The second conclusion that can be drawn is that December is the worst month to launch a theater kickstarter in, with the amoung of failures being almost identical to the amount of successes.
  Based on the goals analysis it can be concluded that the less money you require the more likely you will succeed. However there is an exception to this as projects ranging from a $35,000 goal to a $44,999 one did nearly as well as the cheaper ones, but for the most part, the cheaper your project the better.
  One limitation of this data set is that it doesn't account for the contents of any projects. For example a play could be extremely expensive but be an amazing idea, which could lead to a success. On the inverse if the contents of a play is terrible it could fail even if it was cheap. This however would be very difficult data to obtain for failed projects as it is highly opinionated and we wouldn't have review scores that likely come along with projects that succeeded. 
  An interesting table to create with this dataset would be the outcome based on how long the kickstarter was active for, as it would give us an idea if the length of the kickstarter assists or hinders the success of a project. Another interesting analysis to make would be if whether or not the project was a staff pick had a significant impact on the success of a project.
