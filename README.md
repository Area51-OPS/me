Entry/Exit Tracker
Overview

The Entry/Exit Tracker is a simple web-based application designed to log the movement of individuals (Students, Staff, and Management) in an organization. It allows for tracking entries and exits, storing logs locally, and exporting data to Excel. Access to sensitive logs is password-protected to ensure data security.

Features

Category Selection: Users can select their category: Student, Staff, or Management.

Staff Type Selection: For Staff, users can specify whether they are Teaching or Non-Teaching staff.

Movement Logging: Tracks “Coming” and “Going” movements.

Password-Protected Log Access: Only authorized users can view or export logs.

Local Data Storage: Uses localStorage to persist log data for the current day.

Excel Export: Logs can be exported as .xlsx files using the SheetJS (xlsx) library.

Responsive UI: User-friendly interface with clear input fields and buttons.

Automatic Daily Reset: Warns users to export logs before a new day begins and clears previous logs.

Screens

Category Selection Screen

Choose between Student, Staff, or Management.

Depending on selection, the workflow adapts.

Staff Type Selection Screen

Select Teaching or Non-Teaching staff type (only for Staff category).

Movement Log Screen

Enter Name and Class/Department/Position.

Log “Coming” or “Going” movement.

Log Access Control Screen

Access or export logs with a password.

Set or change password for log security.

Log Viewing Screen

View all recorded entries in a tabular format.

Navigate back to control screen.

How It Works

Category Selection

Students are redirected directly to Movement Log.

Staff select their type before logging movement.

Management can access movement logs and view/export logs.

Movement Logging

User enters their Name and Class/Department/Position.

Clicking Log Entry saves data in local storage.

A unique ID is automatically assigned to each entry.

Log Management

Password protection ensures only authorized users can view/export logs.

Excel export splits logs by category: Students, Staff, Management.

Old-day logs must be exported before new entries can be recorded.

Technology Stack

HTML5: Structure of the web app.

CSS3: Styling and layout.

JavaScript: Application logic and interactivity.

SheetJS (xlsx.js): Excel file creation and download.

LocalStorage: Persistent client-side storage.
Security Notes

Passwords are stored locally in localStorage.

Students and Staff cannot access log viewing/exporting.

Always export logs at the end of the day to avoid data loss.
Limitations

Data persists only in the browser; clearing cache will remove logs.

No backend; multi-user synchronization is not supported.

Excel export depends on the client browser.



Developed as a lightweight, client-side Entry/Exit Tracking tool for educational institutions.
