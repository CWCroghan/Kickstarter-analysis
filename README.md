# Kickstarting with Excel

## Overview of Project

Kickstarter database is an Excel spreadsheet that contains data from historical (2009-2017) Kickstarter efforts. Kickstarter was launched in April 28, 2009 and has the mission of "to help bring creative projects to life" (Reference: https://www.kickstarter.com/about date: 2022).  The base data contains Columns=20 Rows =4114.  The information is organized based on individual projects and includes elements such as type of project, monetary goal, date of launch, and number of doners.  These data can be used to improve future Kickstarter projects by examining the relationship between different elements of the projects and their relationship to the project success.

Refinements of the analysis can be done by limiting the data to projects similar to those proposed by our client.  For example, if the client is interested to launching a new play, then we should limit our analysis to those that are theatrical in type and not include technology or food.

### Purpose

Generate data visualizations based on the Kickstarter spreadsheet to exam the relationship between launch dates, funding goals, and project success.

## Analysis and Challenges

The data were examined for possible trends and relationships with Outcomes.  Outcomes is a categorical data that indicated whether the project was "successful", "canceled", "failed", or "live".  Projects in the data were "successful” (N=2,185), "failed" (N= 1,530), and “canceled" (N=349).  We excluded the 50 "live" projects from our analysis.

The variables that we examined for possibly being related to the Outcomes are the month of launch and the monetary goals of the project.

### Analysis of Outcomes Based on Launch Date

We limited the data for this analysis to project types of “Theater" and outcomes not equal to "live".

The number of projects categorized by outcome is plotted against the Month of the launch.

<img src="https://github.com/CWCroghan/Kickstarter-analysis/blob/main/Theater_Outcomes_Based_on_Launch_Dates.png" alt="Line Plot of Month of Launch vrs Outcomes">

### Analysis of Outcomes Based on Goals

The Goals for each project were categorized into 12 different bins mostly consisting of 5,000 unit ranges.  We examined the possible relationship between project goals and outcomes by plotting the percent of different outcomes against the categorization of goals.

<img src="https://github.com/CWCroghan/Kickstarter-analysis/blob/main/Outcomes_vs_Goals.png" alt="Plot of Goals vrs Outcomes">

## Results

For the analysis of outcomes based on month of launch dates, there is a marked increase in the number of successful projects during the spring and early summer (April, May, Jun).  The peak is in May.  In the other months, the distance between the number of successful and failed projects is fairly constant.  The two outcomes converge in December suggesting that winter is not a good time to start a project.  The number of canceled projects remains consistently low during the entire year.

For the analysis of the outcomes based on goals, the interdependence between the two measures of outcome is clear. Since the number of canceled is consistently low, the percentage of successful projects is approximately 100 - percentage of failed projects.  Setting that issue aside, there is a non-monotonic relationship between percentage of successful and the amount of the initial goal.  There are several inflection points where the percentage of success dips down to below 50% and then goes back up to above 50%.  The highest percentage of successful outcomes are where the goals are quite modest (< 5,000).  While conversely, having a high goal (>= 45,000) results in almost 100% of failed projects.

There are many challenges to the data analysis.  Primarily, the data are not normally distributed.  There are many outliers for example projects that succeeded with only one donor who donated a large sum of money.  In addition, the non-normality of the data limits the analysis to non-parametric and observational determination of any possible trends. One other consideration that should be taken into account when using these data is that these data are historical data collected from 2009 to 2017 and may not be relevant in a post-Covid environment. Since the projects are across several different geographic locations and various monetary units, we should have limited our analysis to one currency or to convert all the currencies to a single unit.

## Recommendations

If pressed to make recommendations on how to proceed with a new Kickstarter project, we would recommend being realistic in your monetary goals and launching your project in the spring.

## Future and Additional analysis

We highly recommend trying to obtain an updated version of the data.  The willingness to support live-events may have drastically changed since the pandemic.  Trying to make predictions based on historical data can be difficult, the additional attitude changes after a major historical event only adds to the possibility of erroneous conclusions.

In conclusion, we recommend that the graphical analysis be backed up with statistical analyses.  The human eye excels as seeing trends even where none exists.  Having hard statistical results would add credence to our findings.
