## Automated-Employee-Time-Off-Management-System


**📌 Introduction**

This project focused on building an automated employee time-off management system using Airtable and Zapier. The goal was to streamline the submission, approval, and tracking of Paid Time Off (PTO) requests, while ensuring accurate leave balances and minimising manual administrative work. Each employee is entitled to 22 working days of PTO annually, with balances resetting automatically at the start of the year.

**🎯 Objectives**

The system was designed to:

- Centralise employee, manager, and leave request data.
- Automate notifications and approval workflows.
- Keep employees updated on the status of their requests.
- Manage leave balances automatically.

**⚙️ Features**

1. Time-Off Application: Employees submit leave requests with details (dates, number of days, notes).
2. Manager Notification: Managers receive automated alerts when a request is submitted.
3. Approval Workflow: Managers approve or reject requests with optional comments.
4. Employee Notification: Employees are notified of the decision in real time.
5. Leave Balance Management: Approved requests deduct from balances, which reset to 22 days annually.

**🛠️ Implementation**
- Airtable: Served as the database to store employee, manager, and leave request records.
- Zapier + Airtable Automations: Managed notifications, approvals, and automatic balance updates.

<img width="1406" height="406" alt="Screenshot 2025-09-17 at 8 59 39 PM" src="https://github.com/user-attachments/assets/a1c62e8d-938e-4999-b192-62a56af8ac02" />





✅ Testing
The system was tested end-to-end to confirm that:
- Requests are captured accurately.
- Notifications are sent at the right stages.
- Approvals and rejections are processed correctly.
- Leave balances update properly.


```mermaid
flowchart TD
    A[Employee Submits Time-Off Request] --> B[Manager Notification via Zapier]
    B --> C{Manager Decision}
    C -->|Approve| D[Update Airtable Record: Approved]
    C -->|Reject| E[Update Airtable Record: Rejected]
    D --> F[Update Employee Leave Balance]
    D --> G[Notify Employee of Approval]
    E --> H[Notify Employee of Rejection]
    F --> I[Reset Balance at Start of Year]
```





The image of the form for the employees to log their leave requests is shown below.

<img width="638" height="389" alt="Screenshot 2025-09-17 at 9 02 34 PM" src="https://github.com/user-attachments/assets/91163f70-bfae-4b0f-9311-d578129e8c69" />

- [Employee Submits Time-Off Request]



<img width="1440" height="760" alt="Screenshot 2025-09-17 at 9 34 31 PM" src="https://github.com/user-attachments/assets/1b568076-0ca1-450c-89ba-58985372e9ae" />


<img width="1051" height="458" alt="Screenshot 2025-09-17 at 9 27 36 PM" src="https://github.com/user-attachments/assets/784f04a9-30ee-456c-9419-5d909fc22018" />

- [Manager Notification via Zapier]



<img width="249" height="116" alt="Screenshot 2025-09-17 at 9 30 56 PM" src="https://github.com/user-attachments/assets/809685ee-6f0a-485a-85a0-fa8b1e87994f" />

- {Manager Decision}




<img width="1413" height="206" alt="Screenshot 2025-09-17 at 9 00 10 PM" src="https://github.com/user-attachments/assets/c67d23d1-1bc8-409a-ac63-dccf2e4fa93c" />

-Update Airtable Record



<img width="998" height="776" alt="Screenshot 2025-09-17 at 9 35 22 PM" src="https://github.com/user-attachments/assets/d1c79fa0-f76a-48db-afc5-5d611cf07fe4" />

- Update Employee Leave Balance





