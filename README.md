# Online Campus Grievance Redressal Portal

## 1. Project Title and Description

A web-based platform that enables students and staff to report campus issues and helps college authorities manage, track, and resolve them efficiently.

## 2. Problem Statement

Lack of a centralized and transparent system for reporting, tracking, and resolving campus grievances efficiently and accountably.

## 3. Target Users

- **Students:** Submit grievances and track their status.
- **Faculty and Staff:** Report campus-related issues.
- **Department Officers:** Manage and resolve assigned grievances.
- **Administrators:** Monitor grievances, manage users, and oversee resolution.

## 4. Existing Solutions

1. **Mangalore University — Student Grievance Management System:** An online platform for university grievance submission and tracking.  
   Link: https://sgms.mangaloreuniversity.ac.in/

2. **DTU Resolve — Delhi Technological University:** A university grievance portal for structured complaint handling.  
   Link: https://grievances.dtu.ac.in/

3. **UGC e-Samadhaan:** A centralized grievance registration and monitoring platform for higher education stakeholders.  
   Link: https://samadhaan.ugc.ac.in/

## 5. Proposed Solution and Innovation

The proposed system centralizes campus issue reporting and provides a structured process for tracking issues until resolution.

**Key innovations:**
- Automatic assignment of grievances to relevant departments.
- Unique grievance IDs and status tracking.
- Deadline-based notifications and escalation.
- Detection of potentially duplicate reports.
- Resolution feedback and basic analytics.

These features aim to improve accountability, transparency, and campus maintenance efficiency.

## 6. MVP Features

1. User login and role-based access.
2. Grievance submission with category, description, and optional photo.
3. Grievance ID generation and status tracking.
4. Department assignment and status updates.
5. Admin dashboard for managing grievances.
6. Deadline tracking and overdue notifications.
7. Resolution feedback and basic analytics.

## 7. Suited Technology Stack

The initial version will use the MERN stack.

| Technology | Purpose |
|---|---|
| MongoDB | Store users, grievances, and status history |
| Express.js | Build backend APIs and handle business logic |
| React.js | Develop interactive user interfaces |
| Node.js | Run the backend server |
| Git and GitHub | Version control and team collaboration |

Additional tools may include JWT for authentication, a file-storage service for evidence uploads, and Chart.js for analytics.

## 8. Draft Architectural Flow Diagram

mermaid
flowchart TD
    A[Student / Staff] --> B[React Frontend]
    B --> C[Submit Grievance]
    C --> D[Node.js + Express Backend]
    D --> E[(MongoDB Database)]
    E --> D
    D --> F[Assign to Department]
    F --> G[Officer Reviews and Resolves]
    G --> E
    D --> H[Status and Notifications]
    H --> B
    B --> I[Admin Dashboard]


### Flow Explanation

1. Students or staff submit a grievance through the frontend.
2. The backend processes the request and stores it in MongoDB.
3. The grievance is assigned to the appropriate department.
4. The officer reviews the issue and updates its status.
5. The frontend displays progress and notifications to users.
6. Administrators monitor grievances through the dashboard.

---
