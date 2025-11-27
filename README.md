📘 Events & Activities Management System (C Program)

A simple, menu-driven Events and Activities Management System written in C.
This program allows users to add, view, search, and delete events and activities using arrays and structures.

This project is ideal for academic assignments, mini-projects, and learning basic C programming concepts.

✅ Features
Event Management

Add new event

View all events

Search event by ID

Delete event by ID

Activity Management

Add new activity

View all activities

Search activity by ID

Delete activity by ID

General Features

Menu-driven interface

Uses arrays to store maximum 100 items

Uses structures for organized data storage

Input handled with fgets() for safety

Simple and beginner-friendly source code

📂 Data Structures Used
Event Structure
struct Event {
    int id;
    char name[50];
    char date[20];
    char venue[50];
};

Activity Structure
struct Activity {
    int id;
    char title[50];
    char time[20];
    char facilitator[50];
};

🖥 How the Program Works
1. Add Event / Activity

User enters:

ID

Name / Title

Date / Time

Venue / Facilitator

The program stores each record in an array.

2. View Events / Activities

Prints all records in a clean list format.

3. Search

Search using ID:

If ID exists → displays record

If not → shows “not found” message

4. Delete

Deletes a record by shifting array elements and reducing the count.

⚙️ Technical Requirements
Software

GCC / MinGW / Clang / MSVC

Any editor (VS Code, CodeBlocks, Dev-C++, Notepad++, etc.)

System

Windows / Linux / macOS

Very low memory usage

Runs in terminal

🏗 Compilation & Execution
Compile
gcc event_activity_system.c -o event_activity_system

Run (Windows)
event_activity_system.exe

Run (Linux/macOS)
./event_activity_system

📜 Program Menu
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

🖼 Sample Output Screenshots (Terminal Text)
➤ Adding an Event
<img width="294" height="149" alt="Screenshot 2025-11-27 102808" src="https://github.com/user-attachments/assets/04b90538-d562-45f1-9214-be242cd84fed" />

Adding an Activity
<img width="339" height="150" alt="Screenshot 2025-11-27 102819" src="https://github.com/user-attachments/assets/c62ad3f8-c3d4-4a9e-84bc-76a0b909b765" />


➤ Viewing  Events

<img width="228" height="172" alt="Screenshot 2025-11-27 102906" src="https://github.com/user-attachments/assets/8c286f17-fcaf-41df-b227-ea71137e301a" />

Viewing Activity

<img width="239" height="168" alt="Screenshot 2025-11-27 102933" src="https://github.com/user-attachments/assets/981a3324-84d2-4ced-aaf4-c7dc4741a652" />

Searching Event 

<img width="289" height="188" alt="Screenshot 2025-11-27 102956" src="https://github.com/user-attachments/assets/21b25182-1279-493c-860c-bbbd562d9a6a" />


➤ Searching Activity

<img width="325" height="190" alt="Screenshot 2025-11-27 103033" src="https://github.com/user-attachments/assets/88fe392d-05f5-4d22-86b7-b4ca695b089a" />


➤ Deleting Event

<img width="291" height="73" alt="Screenshot 2025-11-27 103200" src="https://github.com/user-attachments/assets/aae569c6-57a3-473a-b28e-18cfe0ecb7a1" />


Delete Activity

<img width="318" height="80" alt="Screenshot 2025-11-27 103218" src="https://github.com/user-attachments/assets/1835c668-14ad-4798-ab8b-11c2aa18460f" />

Exit

<img width="246" height="53" alt="Screenshot 2025-11-27 105739" src="https://github.com/user-attachments/assets/1bf492a7-7f91-4ad8-971a-2bd38eecb4c2" />


📑 File Structure
project-folder/
│
├── event_activity_system.c    # Source Code
└── README.md                  # Documentation
