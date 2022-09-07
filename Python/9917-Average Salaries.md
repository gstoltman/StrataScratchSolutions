## Compare each employee's salary with the average salary of the corresponding department.
Output the department, first name, and salary of employees along with the average salary of that department.

```
# Import your libraries
import pandas as pd

# Start writing code
avg_by_dept = employee.groupby('department', as_index=False)['salary'].mean()

empl_w_avg = employee.merge(avg_by_dept, on='department')
#empl_w_avg.rename(columns={'salary_x':'salary', 'salary_y':'avg_salary'})
empl_w_avg[['department', 'first_name', 'salary_x', 'salary_y']]
```
