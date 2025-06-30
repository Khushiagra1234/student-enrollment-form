# Student Enrollment Form (Micro Project)

## Description
This is a web-based Student Enrollment Form built using HTML, Bootstrap, jQuery, and JsonPowerDB. It enables users to **add**, **update**, **delete**, and **reset** student records stored in the cloud database.

The form uses **Roll No** as the primary key to uniquely identify each student. On entering the Roll No, the form checks if the student exists:
- If not found, it allows saving a new student record.
- If found, it loads the existing data for updating or deleting.

## Features
- Form fields: Roll No (primary key), Full Name, Class, Birth Date, Email, Mobile No, Address, Enrollment Date.
- Buttons: Save, Update, Delete, Reset.
- Fields and buttons enable/disable dynamically based on user input and database status.
- Client-side validation ensures no empty fields before saving or updating.
- Uses JsonPowerDB API for all database operations via AJAX calls.
- Local storage used to hold record number (`recno`) for updates and deletes.

## Benefits of Using JsonPowerDB
- Cloud-hosted JSON document database with REST API.
- Simple integration with web apps via HTTP.
- No backend setup required.
- Ideal for quick prototyping and micro projects.

## Release History
- **v1.0.0** - Initial release supporting full CRUD operations on Student records with Roll No as primary key.

## Table of Contents
- [Description](#description)
- [Features](#features)
- [Benefits of Using JsonPowerDB](#benefits-of-using-jsonpowerdb)
- [Release History](#release-history)
- [Usage Instructions](#usage-instructions)
- [Project Status](#project-status)
- [Sources](#sources)

## Usage Instructions
1. Enter **Roll No** and move out of the field (onchange event triggers).
2. If Roll No exists:
   - The form auto-fills the student details.
   - Enables **Update**, **Delete**, and **Reset** buttons.
   - Disables Roll No field.
3. If Roll No does not exist:
   - Enables all fields except Roll No.
   - Enables **Save** and **Reset** buttons.
4. Fill in all fields (Full Name, Class, Birth Date, Email, Mobile No, Address, Enrollment Date).
5. Click **Save** to add a new record or **Update** to modify existing record.
6. Click **Delete** to remove the record.
7. Click **Reset** to clear and prepare the form for new input.

## Project Status
- Fully functional with basic validation and CRUD capabilities.
- Future improvements may include enhanced input validation and UI enhancements.
- ![image](https://github.com/user-attachments/assets/fa8fa685-ff76-4c42-a1b7-6aec8a4b337f)
![image](https://github.com/user-attachments/assets/133cd657-db67-4472-8008-f52209e0e36f)

  
## Sources
- JsonPowerDB API Documentation: https://jsonpowerdb.com
- Bootstrap Framework: https://getbootstrap.com/
- jQuery Library: https://jquery.com/

