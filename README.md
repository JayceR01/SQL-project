# SQL-project
# Applying filters to SQL queries, done during Google Cybersecurity certificate. We were using a setup with files that already had information needed for projects.

# Checking the log_in_attempts table for failed login attempts after 1800
from log_in_attempts 
where login_time > '18:00' and success = false;

# Next, we looked at login attempts that occurred on specific days
from log_in_attempts
where login_date = '2022-05-09' or login_date = '2022-05-05';

# Retrieve login attempts from outside of Mexico 
from log_in_attempts
where country not like 'MEX%';

# Retrieve employees in the marketing department
from employees
where department = 'Marketing' and office like 'East%';

# Retrieve employees in Finance or Sales departments
from employees
where department = 'Sales' or department = 'Finance';

# Retrieve employees not in the IT department
from employees
where not department = 'Information Technology';

# A more in depth explanation of what I was doing and why
[SQL portfolio project.pdf](https://github.com/JayceR01/SQL-project/files/14378439/SQL.portfolio.project.pdf)
