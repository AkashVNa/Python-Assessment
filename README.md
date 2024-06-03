# Python-Assessment
Dataset-- https://docs.google.com/spreadsheets/d/1VP9BE_eI2yl6uUHSm4mGiiwjRdoqCqnkcIjsv5Q2ex4/edit?usp=share_link

Preprocessing- The dataset consisted of two columns(College,Salary) having null values. The column College doesnot play any role in analysis as it is not in our field of consideration so the null values are replaced by a string("Unknown"). The column Salary is important and any filling of null values will lead to incorrect analysis so they are to be dropped however this drop will be delayed until analysis on other columns are carried out. The column(Height) is consisted of month-numerical value, numerical value-month combination. The month is converted to respective numerical value according to the order in the date format which brings us to a numerical value-numerical value format(eg."06-10"). For keeping with the integrity of the values, random values are assigned within some limits. 
    When left numerical value is 05 and right numerical value is less than or equal to 6, values are chosen randomly between 150 and 155.
    When left numerical value is 05 and right numerical value is more than 6, values are chosen randomly between 155 and 160.
    Likewise, when left numerical value is 6, random values between 160 and 170 are inserted and when left value is 7, random values between 170 and 180 is inserted.

Analysis Tasks-
1. Determine the distribution of employees across each team and calculate the percentage split relative to the total number of employees.
2. Segregate employees based on their positions within the company.
3. Identify the predominant age group among employees.
4. Discover which team and position have the highest salary expenditure.
5. Investigate if there's any correlation between age and salary, and represent it visually.

Graphical Representation-
1. Columns Number, Age, Weight, Height, Salary(All the columns which consist of a numerical value) are plotted against each other using pairplot.
2. Countplot to find the count of teams with same number of employees.
3. Pie-chart to find the percentage distribution of employeesof each team.
4. Barplots to find distribution of employees in each position within every team team. For efficient analysis, the map is split into 6 submaps containing 5 teams each.
5. Countplot to find the predominant age in the dataset.
6. Barplot to relate team name vs salary.
7. Barplot to relate  positions within the dataset vs salary.
8. Scatterplot to find the relation between age and salary.
9. Heatmap to check the correlation between age and salary.

Insights gained-
Employee distribution:
  1. 23 out of 30 teams have 15 employees on their payscale which is approximately 77% of total teams.
  2. 2 teams(Orlando magic,Minnesota Timberwolves) have the lowest employee count=14 employees.
  3. New Orleans Pelicans team has largest employee count=19 employees.
  4. Mean, median and mode of employee distribution in teams is approx 15.
  5. The standard deviation of employee distribution in teams is very low=0.98
  6. The distribution of employees in teams are highly dominated by 15.The remaining numbers are roughly a pattern ie 3.33, 3.33*1=3.33, 3.33*2=6.66, 3.33*3=9.99
  7. Brooklyn Nets(SF),Cleveland Cavaliers(C) each have a position with zero employee.
  8. Brooklyn Nets(SG), Memphis Grizzlies(PF) has highest no of players in a specific position=6.

  9. The age group of 24 is the predominant one=47 employees.The age group of 25 doesnt fall far behind(46 employees).
  10. The age of 19 and 39 has minimum presence in the data=2.
  11. The median age is 26.
  12. The standard deviation of age is 4.4
  13. The mean age is approx 27.
   
Salary distribution:
  1. Cleveland Cavaliers has the maximum wage bill=106988689.
  2. Philadelphia 76ers has the lowest wage bill=30992894.
  3. Lowest team salary is approx 70% less than the highest team salary.
  4. The mean team salary is 72026146.
  5. The median team salary is 71727048.5
  6. The standard deviation in team salary is 15118297.5

  7. Position C has highest salary among positions.
  8. Position SG has the lowest salary.
  9. Maximum variation between salary related to positions is at 15% approximately.
  10. Age and salary has almost no correlation with correlation coefficient=0.214
