# ENG_315_GroupProject-The_Compensated
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
