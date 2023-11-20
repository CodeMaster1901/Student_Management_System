# Student_Management_System
The Student Management System is a web application developed using the Flask web framework, SQLAlchemy for database interactions, and Flask-Login for user authentication. The system allows users to manage student-related information, such as student details, attendance, departments and triggers.

## Key Components

#### Database Models:

Test: Represents a test entity with attributes like id, name, and email.

Department: Represents a department entity with attributes like cid (department ID) and branch.

Attendance: Represents attendance information with attributes like aid, rollno, and attendance.

Trig: Represents triggers with attributes like tid, rollno, action, and timestamp.

User: Represents user information for authentication with attributes like id, username, email, and password.

Student: Represents student details with attributes like id, rollno, sname, sem, gender, branch, email, number, and address.

#### Routes and Views:

/: Displays the home page. 

/studentdetails: Shows student details, including department-wise student counts and total student count.

/triggers: Displays triggers.

/department: Allows adding new departments.

/addattendance: Enables adding attendance records for students.

/search: Provides a search functionality based on the student's roll number.

/delete/<string:id>: Allows deleting a student record.

/edit/<string:id>: Allows editing student details.

/signup: Handles user registration.

/login: Manages user login.

/logout: Handles user logout.

/addstudent: Allows adding new student records.

/test: Checks the database connection.

#### User Authentication:

User registration and login are implemented using Flask-Login.
Passwords are hashed using generate_password_hash and checked using check_password_hash.

#### Database Interaction:

SQLAlchemy is used to interact with the MySQL database.
Various queries and procedures are executed to fetch and manipulate data.

#### Flash Messages:

Flash messages are used for providing feedback to users, such as success messages, warnings, and errors.

#### Dependencies:

Flask, Flask-Login, and SQLAlchemy are major dependencies.
MySQL is used as the database.
Overall, the system provides a platform for managing student-related data, attendance, and triggers, with user authentication and proper feedback mechanisms.

To run this project we first need to download the required modules specified in the requirements.txt file. Open cmd in the project directory and run:
```
pip install -r requirements.txt
```

To execute the project run:
```
python run.py
```

Copy the url to a new tab in Google Chrome and the project will run



