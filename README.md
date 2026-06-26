# 🛡️ FRANK Cybersecurity Awareness Chatbot

## PROG6221 Programming 2A – Part 3 (POE)

### Author

**Keatlegile Sanele Mhlanga**

Rosebank College

2026

---

# Project Overview

FRANK (Friendly Responsive Assistant for Network Knowledge) is a GUI-based cybersecurity awareness chatbot developed using **C#**, **WPF**, and **XAML**.

The application combines the functionality developed throughout Parts 1, 2 and 3 of the POE into one complete application. It assists users by providing cybersecurity advice, managing cybersecurity-related tasks, setting reminders, offering an interactive quiz, simulating Natural Language Processing (NLP), and maintaining an activity log.

---

# Features

## 💬 Cybersecurity Chatbot

The chatbot can answer questions about:

* Phishing
* Password Safety
* Malware
* Privacy
* Online Scams
* Suspicious Links
* Safe Browsing
* Two-Factor Authentication

Additional chatbot features include:

* Greeting users
* Sentiment detection
* Keyword recognition
* Randomised responses
* Favourite topic memory
* Conversation history

---

# ✅ Task Assistant

The Task Assistant allows users to manage cybersecurity tasks.

### Features

* Add new tasks
* Add task title
* Add task description
* Add reminder dates
* View all tasks
* Mark tasks as completed
* Delete individual tasks
* Delete all tasks

### Example Commands

```text
Remind me to update my password in 7 days

Remind me to enable two-factor authentication tomorrow

Remind me to review my privacy settings on 30 June 2026

Show tasks

View all tasks

Delete task update my password

Delete all tasks

Complete task update my password
```

---

# 🗄️ Database Integration

The Task Assistant uses a SQL database to permanently store task information.

The database supports the following CRUD operations:

* Create Tasks
* Read Tasks
* Update Completed Tasks
* Delete Tasks

The following information is stored:

* Task Title
* Task Description
* Due Date
* Completion Status

Tasks are automatically loaded when the application starts.

---

# 🎮 Cybersecurity Quiz

The chatbot includes an interactive cybersecurity quiz.

### Quiz Features

* GUI-based interface
* More than 10 cybersecurity questions
* Multiple Choice Questions
* True / False Questions
* Immediate feedback
* Score tracking
* Final score display

### Topics Covered

* Phishing
* Password Safety
* Malware
* Online Scams
* Privacy
* Safe Browsing
* Two-Factor Authentication
* Social Engineering

### Start the Quiz

Type any of the following:

```text
quiz

start quiz

play quiz

begin quiz

cybersecurity quiz
```

---

# 🧠 Natural Language Processing (NLP)

The chatbot recognises multiple ways of asking for the same action.

Examples include:

```text
Remind me to update my password

Add task to review privacy settings

Can you remind me to enable 2FA?

Show tasks

Delete task password update

Start quiz

Show activity log

What have you done for me?
```

The chatbot uses:

* Keyword Detection
* String.Contains()
* String Manipulation
* Date Recognition
* Basic NLP Simulation

---
# Example Commands to Test FRANK

The following commands can be entered into the chatbot to test all implemented features.

---

## General Cybersecurity Questions

- What is phishing?
- Tell me about phishing
- Explain phishing
- What is password safety?
- Tell me about passwords
- What is malware?
- Tell me about malware
- What is privacy?
- What is a scam?
- What are suspicious links?
- How are you?
- What can I ask you?
- What is your purpose?

---

## Sentiment Detection

- I am worried about scams
- I am scared
- I am happy
- I am frustrated
- I am angry

---

## Memory Feature

Store information:

- My favorite topic is privacy
- My favorite topic is phishing
- My favorite topic is password safety

Recall information:

- What is my favorite topic?
- Tell me my favorite topic
- Favorite topic

---

## Task Assistant

### Create Tasks

- Remind me to update my password in 7 days
- Remind me to enable two-factor authentication tomorrow
- Remind me to review my privacy settings next week
- Remind me to back up my files on 30 June 2026
- Remind me to do research on phishing in 3 days
- Add task to check suspicious emails tomorrow
- Can you remind me to change my password in 5 days?

### View Tasks

- View tasks
- Show tasks
- My tasks
- List tasks
- List all tasks

### Delete Tasks

Delete a single task:

- Delete task update my password
- Remove task phishing
- Delete task backup

Delete all tasks:

- Delete all tasks
- Remove all tasks

### Complete Tasks (if implemented)

- Complete task update my password
- Mark task update my password as completed
- Finish task update my password

---

## Cybersecurity Quiz

Start the quiz using any of the following:

- Quiz
- Start quiz
- Begin quiz
- Cybersecurity quiz
- I want to take a quiz
- Test my cybersecurity knowledge
- Give me a quiz

Answer using:

- A
- B
- C
- True
- False
- T
- F

---

## NLP Simulation

The chatbot recognises different ways of asking for the same action.

Examples:

- Add task to update my password
- Can you remind me to enable 2FA?
- Remind me to review my privacy settings tomorrow
- Show my tasks
- List all tasks
- Delete task phishing
- Remove all tasks
- Start quiz
- Show activity log
- What have you done for me?

---

## Activity Log

View logged actions using:

- Show activity log
- Activity log
- Show recent actions
- What have you done for me?
- Show log
- View activity log

The activity log records events such as:

- User messages
- Bot responses
- Tasks added
- Tasks deleted
- Tasks completed
- Reminders created
- Quiz started
- Quiz completed
- NLP commands recognised

---

## Random Response Feature

Ask the same question multiple times to see different responses.

Examples:

- Tell me about phishing
- What is phishing?
- Password tips
- Tell me about passwords

---

## Database Feature

Once the SQL Server database is configured, test the following:

1. Create a new task.
2. Close the application.
3. Reopen the application.
4. Verify that the task is still available.
5. Mark the task as completed.
6. Delete the task.
7. Verify that all changes are reflected in the database.

---

## Expected Features Demonstrated

✔ GUI Chatbot  
✔ Cybersecurity Knowledge Base  
✔ Sentiment Detection  
✔ Memory Feature  
✔ Random Responses  
✔ NLP Simulation  
✔ Task Assistant  
✔ Reminders  
✔ CRUD Task Management  
✔ Activity Log  
✔ Cybersecurity Quiz  
✔ Database Integration (SQL Server)

# 📋 Activity Log

The chatbot records important system events including:

* User messages
* Chatbot responses
* Task creation
* Reminder creation
* Task completion
* Task deletion
* Quiz started
* Quiz completed
* NLP commands recognised

### View Activity Log

Type:

```text
Show activity log

Show recent actions

What have you done for me?
```

The chatbot displays the most recent activities.

---

# 💻 Software Requirements

Install the following software before running the project:

* Visual Studio 2022
* .NET Framework
* SQL Server LocalDB / SQL Server Express
* SQL Server Object Explorer (Visual Studio)

---

# ⚙️ How to Run the Project

1. Clone or download the GitHub repository.
2. Open the solution in Visual Studio.
3. Restore any required NuGet packages.
4. Build the solution.
5. Press **F5** or click **Start**.
6. The chatbot application will open.

---

# 🗄️ Database Setup

1. Open **SQL Server Object Explorer** in Visual Studio.

2. Create a new database named:

```text
studentData
```

3. Create a **tblTasks** table.

Suggested table structure:

| Column      | Data Type                   |
| ----------- | --------------------------- |
| Id          | INT (Primary Key, Identity) |
| Title       | NVARCHAR(255)               |
| Description | NVARCHAR(MAX)               |
| DueDate     | DATETIME                    |
| IsCompleted | BIT                         |

4. Update the application's connection string if necessary.

5. Run the application.

---

# 📂 Project Structure

```text
FRANK_CHATBOT_PART2
│
├── chatbot.xaml
├── chatbot.xaml.cs
├── MainWindow.xaml
├── MainWindow.xaml.cs
├── Session.cs
├── TaskItem.cs
├── QuizQuestion.cs
├── App.xaml
├── App.xaml.cs
├── README.md
└── Database Scripts
```

---

# 🛠️ Technologies Used

* C#
* WPF (Windows Presentation Foundation)
* XAML
* SQL Server
* ADO.NET
* .NET Framework

---

# 🚀 GitHub Repository

This repository demonstrates continuous development through multiple commits and tagged releases.

Minimum repository requirements:

* Six or more meaningful commits
* Three or more releases/tags
* Complete project source code
* README file
* Database setup instructions

---

# 🎥 Video Demonstration

**YouTube (Unlisted) Video Link**

Replace this section with your video link before submission.

Youtube link:

```text
https://youtu.be/_OkLc4OlZ5M
```
Github link : 
```text
https://github.com/sanele02/FRANK-Cybersecurity-Assistant-Part-3-
```	
---

# Important Notes

* The application is GUI-based using WPF.
* The chatbot combines Parts 1, 2 and 3 into one application.
* Internet access is not required.
* SQL Server must be installed before running the database features.
* Ensure the database connection string matches your SQL Server instance.

---

# License

This project was developed for educational purposes as part of the **PROG6221 Programming 2A Practical Object-Oriented Exercise (POE)** at Rosebank College.

© 2026 Keatlegile Sanele Mhlanga
