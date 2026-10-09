
# RaceDay RESTful API - Part 2

[![Build and Test Pipeline](../../actions/workflows/dotnet-ci.yml/badge.svg)](../../actions)

## 📌 Project Overview
**RaceDay** is a RESTful API built with **ASP.NET Core Web API** using the **Code-First** approach with **Entity Framework Core** and **SQL Server**. The system serves as the central backend powering event creation, category management, participant enrolments, and result tracking for athletic events.

This API strictly enforces **Role-Based Access Control (RBAC)** via session management and stores hashed user passwords using BCrypt.

---

## 👥 User Roles & Permissions

The system supports two primary user roles:

### 1. Organiser
* **Event Management:** Can create, update, and delete events.
* **Category Management:** Can create, update, and delete categories attached to events.
* **Enrolment Oversight:** Can view all participant enrolments for their events.
* **Result Capture:** Can record and correct participant finish times and positions.

### 2. Participant
* **Browsing:** Can view upcoming events, event details, categories, and event leaderboards.
* **Profile Management:** Can view and update their personal account profile.
* **Enrolments:** Can enrol into specific event categories and view/cancel their active enrolments.
* **Results:** Can view their personal race history and finish times.

---

## 🚀 Getting Started & Local Setup Instructions

### Prerequisites
* [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
* [SQL Server Express / LocalDB](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
* [Visual Studio 2022](https://visualstudio.microsoft.com/) OR [Visual Studio Code](https://code.visualstudio.com/)

### Step-by-Step Setup

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)<YOUR_GITHUB_USERNAME>/<YOUR_REPOSITORY_NAME>.git
   cd <YOUR_REPOSITORY_NAME>
