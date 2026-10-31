# ENG 315 Group Project-The Compensated (sub-task-1)

**Objective and Motivation(sub-task-2):** We are analyzing the veteran’s association's (VA) total distribution of compensated funds throughout the fiscal year of 2025, excluding the 149,077 recipients who were taken off the program during that year. The motivation behind this program is to understand how VA benefits are spread throughout our country. This dataset gives us an insight into what countries receive the greatest number of benefits, what kind of recipients there are, including biological data such as age or gender, and how much certain recipients are receiving. The three questions we are asking are which state has the most US disability compensation recipients, what is the ratio of male to female veteran disability compensation, and what is the distribution of compensation over age groups of 17-44, 45-64, and 65 + year old recipients?

### Sophia: Male-to-Female Ratio of Disability Compensation Recipients

**Question:** What is the ratio of male to female veterans receiving disability compensation?

**Method:** Use the FY 2025 Disability Compensation Recipients by County dataset to calculate male and female recipient totals, their percentages, and the male-to-female ratio. Check for missing or suppressed counts without treating blanks as zeros, and avoid counting summary totals twice.

**Statistical Test:** Use a chi-square goodness-of-fit test to determine whether the observed male and female recipient counts differ from an expected distribution. Select and justify the expected proportions before testing.

- **Null hypothesis:** The recipient proportions match the selected expected male/female proportions.
- **Alternative hypothesis:** The recipient proportions differ from the selected expected proportions.
- **Significance level:** 0.05. A p-value below 0.05 indicates a statistically significant difference.

**Metrics:** Male and female totals, percentages, male-to-female ratio, chi-square statistic, and p-value.

**Tools:** Python with pandas for organizing and calculating the data, SciPy’s `chisquare()` function for the test, and matplotlib for visualization.

**Plot:** A grouped bar graph comparing observed and expected male and female recipient counts.

### Ryan: State with highest total disability compensation recipients

**Question:** Which state has the most US disability compensation recipients? 

**Method:** The task required to complete the question is to make a code that can process the columns containing the number of recipients within each country and then summarize the total numbers between countries within a designated state. This process requires using pandas, which will allow the exported csv file’s column values to be read. Within this csv file, there are U.S territories which should not be accounted for, this is included in a different column comparatively to state/counties but should not be inputted in. For the correctly interpreted value, there is a column in the csv file labeled, “Total: Disability Compensation Recipients”, this shows the total value of recipients within a county. This must be expanded and summed together in groups of respected states. There is a group row containing each state, by grouping together the states and summing their combined county values, we will arrive at each state’s total disability compensation recipients. From this point on, we can take the total raw count of each state and have the code display the highest valued state in terms of total recipients.

**Test:** Creating a sorted list in ascending order of total number of disability recipients, and revealing the state with the highest value

- **Pandas:** Allows for code to read data points derived from columns/ rows
  
- **Column selection:** Selecting Total: Disability Compensation Recipients to derive total number of disability recipients in each county
  
- **State restriction:** group states together to remove U.S territories from total set
  
- **Total Sum for each state:** sums total number of recipients in each state
  
- **Sort:** Sorting will create a list from the states in values of their total sum showing the highest valued state in terms of # of disability recipients
  
### Eduardo: Age Distribution of Disability Compensation Recipients

**Question:** How are US disability compensation recipients distributed across age groups?

**Method:** Utilizing the Disability Compensation Recipients database we assigned ourselves and using the NumPy and pandas libraries within python, calculate the total recipients of each age group (17-44, 45-64 and 65+), contrast them with the overall total recipients and calculate percentages for each of the age groups compared to the total.

**Statistical Test:** Use a chi-square goodness-of-fit test to determine if the results of the calculation fit our expected output. Said previous output can be determined manually with a variable and justified.

- **Null hypothesis:** The recipient proportions match the selected expected age variety proportions.
- **Alternative hypothesis:** The recipient proportions are skewed from the expected results.
- **Significance level:** 0.05. A p-value below 0.05 indicates a statistically significant difference.      

**Metrics:** Overall total recipients, the total per each age group, the percentage of each agegroup compared to the total, chi-square statistic, and p-value.

**Tools:** Python with pandas for organizing and calculating the data, SciPy’s `chisquare()` function for the test, and matplotlib for visualization.

**Plot:** A Pie graph comparing the percentages of each age group

#Implementation Details (sub-task-3 and sub-task-4):

In this section, you will go over the methods (with metrics, tools, and plots) to be used to answer the questions. This is the main body of the repo.
The following also be added in the coming phases
Add any screenshot that you feel is necessary to show the project's complexity, such as block diagrams, snippets of the code that carries explicitly a method, the top-level code, etc.
#Results(sub-task-6)Answers to the Questions:
Just have the title as a placeholder to be populated later
#Conclusions(sub-task-7) :
Just have the title as a placeholder to be populated later
#Actions that need to be completed:
Just have the title as a placeholder to be populated later

