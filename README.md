MEDTRACK SYSTEM INSTALLATION PROCESS 

This file outlines the requirements and steps involved in running the MedTrack system on your machine.
MedTrack is a healthcare management system designed to manage patient records, medical histories, appointments, and prescriptions.

Programming Language: Python (version 3.x)

### Prerequisites:
Ensure that the following softwares and libraries are installed:
- MySQL Database: MedTrack requires MySQL to store and manage data. Ensure that MySQL is installed and running on your system.
  - MySQL can be downloaded at this link: https://dev.mysql.com/downloads/
  - Expected installation directory for MySQL Database
    - Windows: C:\Program Files\MySQL\MySQL Server 8.0
    - macOS: /usr/local/mysql
    - Linux: /etc/mysql
  - Create a database named med_track, set up the tables according to the schema provided in the project, and ensure MySQL is running and accessible
- Python (version 3.x): The project is written in Python and the necessary Python libraries must be installed as well.
  - Python (version 3.x) can be downloaded at this link: https://www.python.org/downloads/
  - Expected installation directory for Python
    - Windows: C:\Python3x
    - macOS: /usr/local/bin/python3
    - Linux: /usr/bin/python3
  - Ensure Python is running and accessible
- Python Libraries: The following Python libraries are required for the MedTrack project.
  - pymysql: a library to interact with MySQL databases
    - To install this library, you can run the following: pip install pymysql
    - To import the library, this line of code can be used: import pymysql
  - matplotlib: a library for creating visualization in Python
    - To install this library, you can run the following: pip install matplotlib
    - To import this library, this line of code can be used: import matplotlib.pyplot as plt 

### Running the Application:
- Run this application in a python application: finalprjcode.py
- Enter your MySQL username and password correctly (if wrong then try again)
- Enter whether if you are a doctor or pharmacist
- Enter your username and password for the MedTrack system
- The specified port in the code is 3308; change the port to 3306 if there is a port issue

## Choosing from the Main Menu:
- The options are listed as the following:
  - 1: Add patient details and medical history (if you choose to do this action, you must input values - e.g. DOB, name, and address)
    - This will make the system assign a unique patient ID to the entry
  - 2: Update patient details (if you choose to do this action, you must input a patient ID to select a patient and input updates to a patient's details)
  - 3: Update medical history (if you choose to do this action, you must input a patient ID to select a patient and input updates to a patient's medical history details)
  - 4: Remove patient details and medical history (if you choose to do this action, you must input a patient ID and type “yes” to confirm this decision)
  - 5: View all patient details (if you choose to do this action, all records in the patient table are retrieved and displayed)
  - 6: View patients' medical history (if you choose to do this action, all records in the medical_history table are retrieved and displayed)
  - 7: Schedule an appointment (if you choose to do this action, you must input a patient ID, doctor NPI, date, time, location, and appointment reason)
  - 8: Cancel an appointment (if you choose to do this action, you must input a patient ID, doctor NPI, date, and time)
  - 9: View appointments (if you choose to do this action, all appointment records are retrieved and displayed)
  - 10: Create a prescription (if you choose to do this action, you must input a patient ID, medication name(s), dosage, pharmacy NPI, and expiration date)
  - 11: View prescriptions (if you choose to do this action, all prescription records are retrieved and displayed)
  - 12: Filter prescription details by prescription ID (if you choose to do this action, you must input a specific prescription ID)
  - 13: Find expired prescriptions (if you choose to do this action, all expired prescriptions are retrieved and displayed)
  - 14: Refill expired prescriptions (if you choose to do this action, you must input an expired prescription ID and pharmacist NPI)
  - 15: View patient age distribution (if you choose to do this action, a pie chart showing the percentages of patients part of each age group will be displayed)
  - 16: View patient insurance provider distribution (if you choose to do this action, a bar chart showing the number of patients on each insurance company will be displayed)
  - 17: Exit (more information on this option is listed below)

### Exiting the Application:
- If you would like to disconnect and exit, choose option 17 from the menu (by typing "17")
- This will close the connection to the database and the program will end
