# Student_Management_System
The Student Management System is a web application developed using the Flask web framework, SQLAlchemy for database interactions, and Flask-Login for user authentication. The system allows users to manage student-related information, such as student details, attendance, departments and triggers.

# Key Components

## Database Models:

  **1. Test:** Represents a test entity with attributes like id, name, and email.

  **2. Department:** Represents a department entity with attributes like cid (department ID) and branch.

  **3. Attendance:** Represents attendance information with attributes like aid, rollno, and attendance.

  **4. Trig:** Represents triggers with attributes like tid, rollno, action, and timestamp.

  **5. User:** Represents user information for authentication with attributes like id, username, email, and password.

  **6. Student:** Represents student details with attributes like id, rollno, sname, sem, gender, branch, email, number, and address.

## Routes and Views:

  **/:** Displays the home page. 

  **/studentdetails:** Shows student details, including department-wise student counts and total student count.

  **/triggers:** Displays triggers.

  **/department:** Allows adding new departments.

  **/addattendance:** Enables adding attendance records for students.

  **/search:** Provides a search functionality based on the student's roll number.

  **/delete/<string:id>:** Allows deleting a student record.

  **/edit/<string:id>:** Allows editing student details.

  **/signup:** Handles user registration.

  **/login:** Manages user login.

  **/logout:** Handles user logout.

  **/addstudent:** Allows adding new student records.

  **/test:** Checks the database connection.

## User Authentication:

User registration and login are implemented using Flask-Login.
Passwords are hashed using generate_password_hash and checked using check_password_hash.

## Database Interaction:

SQLAlchemy is used to interact with the MySQL database.
Various queries and procedures are executed to fetch and manipulate data.

## Flash Messages:

Flash messages are used for providing feedback to users, such as success messages, warnings, and errors.

## Dependencies:

Flask, Flask-Login, and SQLAlchemy are major dependencies.
MySQL is used as the database.
Overall, the system provides a platform for managing student-related data, attendance, and triggers, with user authentication and proper feedback mechanisms.

# Getting Started

To run the project follow these steps:

  **1. Clone the repository:**

  ```
  git clone https://github.com/AbhayKamath03/Student_Management_System.git
  ```


  **2. Install Dependancies:**
  ```
  pip install -r requirements.txt
  ```


  **3. Run the application:**
  ```
  python run.py
  ```


  **4. Access the System:** Open your web browser and navigate to http://127.0.0.1:5000 to access the Student Management System



