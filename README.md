Name:MANOJ KENGALAGUTTI
COMPANY NAME:CODTECH IT SOLUTIONS
ID:CT6WDS2472
DOMAIN:PYTHON
DURATION:NOV25 TO JAN 6 
MENTOR:NEELA SANTOSH KUMAR

Project Overview: Student Grades Management System
The Student Grades Management System is a Python-based application designed to help educators, administrators, or institutions efficiently manage and track student grades across multiple subjects. The system enables users to input, store, update, and retrieve student grades, calculate average grades, assign letter grades, compute GPAs, and maintain a record of weighted averages for various assignments or subjects.

Core Features:
User-Friendly Interface:

The system interacts with users via the terminal (command-line interface). The program presents a menu with clear options, allowing users to easily navigate through the different features of the application.
Input Grades for Multiple Subjects:

Users (teachers or administrators) can input grades for multiple subjects or assignments for each student.
Users can specify the weight (percentage) of each subject to calculate the weighted average, which is especially useful for cases where some subjects or assignments carry more importance than others.
Calculating Grades:

Average Grade: The program computes the simple average of all grades entered by the user.
Letter Grade: Based on the average grade, the system assigns a letter grade (A, B, C, etc.), following typical grading standards (e.g., 90+ is A, 80-89 is B, etc.).
GPA: The system calculates a Grade Point Average (GPA) based on the numeric average. This is commonly used in educational institutions to represent overall performance.
Weighted Average: Users can also input weights for each subject or assignment. The program calculates a weighted average based on the weights provided by the user, which adjusts the final score based on the relative importance of each subject.
Data Persistence:

The system stores all the student data (grades, subjects, letter grades, GPAs, etc.) in a JSON file (students.json). This ensures that the data is saved between sessions, and users can retrieve student records even after restarting the program.
The program can load student data when started and save updates to the file when grades are entered or updated.
Student Management:

The system supports managing multiple students' records.
Users can view the grades, average grade, letter grade, GPA, and weighted average of any student stored in the system.
The program also allows updating a student's grades if needed.
Interactive Menu System:

The program presents an interactive menu to the user, providing options to:
Add or update grades for a student.
View grades for a specific student.
View a summary of all students.
Exit the system.
Flow of the Program:
Starting the Program:

When the program starts, it loads any existing student data from the students.json file (if it exists) into memory.
If no data is available, it will create a new file when data is saved.
Main Menu:

Users are presented with a set of options:
Add/Update Student Grades: This option allows the user to input or update grades for a specific student. The user provides the student's name, subjects, grades, and weights.
View Student Grades: Allows the user to view detailed grades for a specific student, including their average grade, letter grade, GPA, and weighted average.
View All Students: Displays a list of all students, showing a brief summary of each student's grades, average, letter grade, and GPA.
Exit: Exits the program and saves all the data.
Data Handling:

After a student's grades are input, the program computes the average grade, letter grade, GPA, and weighted average (if applicable).
The results are displayed to the user, and the student's data is saved in the students.json file.
Data Persistence (Saving & Loading):

Whenever data is updated (such as adding new grades or modifying existing ones), the program saves the student data back to the JSON file. This allows users to persist the data between sessions.
When the program is restarted, it loads the stored data so that the user can continue managing grades without losing any information.
Use Cases and Application:
Educational Institutions: This system can be used by teachers or administrators to keep track of students' performance in various subjects over time. It can generate reports that summarize the student's performance for individual assignments, overall course grades, and even provide insights into the GPA.

Online Learning Platforms: The system can be adapted for online learning platforms to allow educators to assess and track students' progress across multiple modules and assignments.

Private Tutors: Tutors can use the system to track the progress of their students in different subjects and provide performance summaries, including letter grades and GPA calculations.

Technical Details:
File Handling: The program uses JSON for data storage. This lightweight format allows easy saving and loading of complex data (like student grades) in a structured way.
User Interface: The application is designed as a command-line interface (CLI), where the user interacts with the program by choosing options from a menu.
Grade Calculations: The program handles basic numerical computations (average grades), but also includes more advanced features like weighted averages, letter grades, and GPA calculation.
Example Walkthrough:
Start the Program:

Upon launching, the system will present the following options to the user:

sql
Copy code
Options:
1. Add/Update Student Grades
2. View Student Grades
3. View All Students
4. Exit
Add/Update Student Grades:

The user selects option 1 to add or update a student’s grades. The system prompts for the student’s name, subjects, grades, and their respective weights.
Once entered, the system will calculate the average, letter grade, GPA, and weighted average and save the information.
View Student Grades:

The user selects option 2 and enters the student's name. The program then displays the grades, average grade, letter grade, GPA, and weighted average for that student.
View All Students:

Option 3 displays all students stored in the system with a summary of their grades.
Exit the Program:

The user can choose option 4 to exit the program, at which point all data is saved.
Example Output:
yaml
Copy code
Welcome to the Student Grades Management System!

Options:
1. Add/Update Student Grades
2. View Student Grades
3. View All Students
4. Exit

Enter your choice: 1
Enter the student's name: John Doe
How many subjects/assignments for John Doe? 3
Enter name for subject 1: Math
Enter grade for Math: 85
Enter weight (in %) for Math: 40
Enter name for subject 2: Science
Enter grade for Science: 90
Enter weight (in %) for Science: 30
Enter name for subject 3: History
Enter grade for History: 75
Enter weight (in %) for History: 30

--- Results ---
Student: John Doe
Subjects: ['Math', 'Science', 'History']
Grades: [85.0, 90.0, 75.0]
Average Grade: 83.33
Letter Grade: B
GPA: 3.00
Weighted Average: 83.33%

John Doe's grades have been saved successfully.
Conclusion:
The Student Grades Management System is a powerful tool for managing student grades and performance over time. By supporting features like GPA calculation, weighted averages, and grade persistence, it can be highly useful for educational institutions, private tutors, and online learning platforms. The system is designed to be simple to use while being flexible enough to accommodate additional features in the future.
