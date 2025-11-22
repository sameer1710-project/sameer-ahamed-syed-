1. Abstract

The Events / Activities Management System is a simple, menu-driven, terminal-based application developed in C to efficiently organize and track events and activities. The system provides essential features such as adding new events or activities, viewing stored records, searching entries by their ID, and deleting outdated or unwanted records. Data is maintained using in-memory structures (arrays) and managed through user-friendly menus, making the program ideal for beginners, students, and small organizations.
This project demonstrates fundamental C programming concepts including structures, arrays, input handling, control flow, and basic data organization. It provides a lightweight and accessible tool for managing event-related information within a command-line environment.

2. Features of the Program
✔ Event Management

Add new event details (ID, name, date, venue)

View all stored events

Search event by ID

Delete event from the list

✔ Activity Management

Add new activity details (ID, title, time, facilitator)

View all stored activities

Search activity by ID

Delete activity from the list

✔ System Features

Fully terminal-based CLI program

Beginner-friendly code structure

Clear, user-guided menu

Validates and handles basic user input

Stores up to 100 events and 100 activities

Uses C structures and arrays for data management

3. Technical Requirements
3.1 System Requirements

Operating System: Windows / Linux / macOS

Command-line / Terminal

Minimum RAM: 4 MB

Minimal disk space (no file storage required)

3.2 Software Requirements

C Compiler: GCC / Clang / MSVC / MinGW

Text editor or IDE (VS Code, Code::Blocks, Dev-C++, etc.)

3.3 Programming Requirements

Language: C

Supported Standards: C89 / C99 / C11

Standard Libraries Used:

#include <stdio.h>
#include <string.h>

3.4 Data Handling Requirements

All data stored temporarily in arrays

Maximum of 100 events and 100 activities

No external files required

3.5 Compilation Requirements

Code must compile without errors

Recommended compilation flags:

gcc events_activities.c -o management -Wall

4. Functional Requirements
4.1 User Interface

Fully menu-driven

Clear text-based options

Accepts numeric and text inputs

Displays confirmation and error messages

4.2 Event Operations

Add Event → Store event details

View Events → Display all events

Search Event → Find event using its ID

Delete Event → Remove entry from list

4.3 Activity Operations

Add Activity → Store activity details

View Activities → Display activity list

Search Activity → Find activity using ID

Delete Activity → Remove activity

4.4 Program Flow

Uses an infinite loop that displays menu until user selects Exit

Each option returns user to main menu

Prevents overflow when maximum storage is reached

Ensures smooth navigation

5. How to Run the Program
Step 1: Save the Code

Save your C program as:

events_activities.c

Step 2: Compile

Linux/macOS:

gcc events_activities.c -o management


Windows (MinGW):

gcc events_activities.c -o management.exe

Step 3: Run

Linux/macOS:

./management


Windows:

management.exe

6. Example Screenshots (Conceptual)
1. Main Menu
==== Events / Activities Management System ====
1. Add Event
2. Add Activity
3. View Events
4. View Activities
5. Search Event
6. Search Activity
7. Delete Event
8. Delete Activity
9. Exit
Enter your choice:

2. Add New Event
Enter Event ID: 101
Enter Event Name: Science Fair
Enter Event Date: 20/12/2024
Enter Event Venue: Auditorium
Event added successfully!

3. View Events
--- Events List ---
ID: 101
Name: Science Fair
Date: 20/12/2024
Venue: Auditorium

4. Search Activity
Enter Activity ID to search: 3

Activity Found:
ID: 3
Title: Debate Practice
Time: 4:00 PM
Facilitator: Mr. Smith

5. Delete Event
Enter Event ID to delete: 101
Event deleted successfully!

6. Exit
Exiting program...

✔ Documentation Completed

This is the full matching format you requested — exactly like the Patient Management System but adapted for your Events / Activities Management System code.
