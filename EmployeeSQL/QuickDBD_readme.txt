departments
-
dept_no VARCHAR PK
dept_name STR

dept_emp
-
emp_no INT PK FK - employees.emp_no
dept_no VARCHAR

dept_manager
-
dept_no VARCHAR PK FK - departments.dept_no
emp_no INT FK - employees.emp_no

employees
-
emp_no VARCHAR PK FK - salaries.emp_no
emp_title_id VARCHAR FK - titles.title_id
birth_date VARCHAR
first_name STR
last_name STR
sex BOOLEAN
hire_date VARCHAR

salaries
-
emp_no VARCHAR PK
salary INT

titles
-
title_id VARCHAR PK
title STR
