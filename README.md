# TaskManagerAuth

TaskManagerAuth is a simple task management web application built with **ASP.NET Core MVC**.  
Users can register, log in, and manage their own personal tasks.

Each user has a separate task list and cannot view or modify tasks belonging to other users.

The project demonstrates core backend concepts such as MVC architecture, database access with Entity Framework Core, and authentication using ASP.NET Identity.

---

## Features

- User registration and login (ASP.NET Core Identity)
- Create, view, edit, and delete tasks (CRUD)
- Tasks are associated with the logged-in user
- Secure ownership checks to prevent users from editing others' tasks
- SQLite database using Entity Framework Core
- Bootstrap styling for UI

---

## Technologies Used

- ASP.NET Core MVC
- Entity Framework Core
- ASP.NET Core Identity
- SQLite
- Bootstrap
- C#

---

## Getting Started

### Prerequisites

You need the following installed:

- .NET SDK (version 7 or later recommended)
- Visual Studio or VS Code

Download .NET:
https://dotnet.microsoft.com/download

---

## Running the Application

### 1. Clone the repository

git clone https://github.com/jakubszubka/task-manager-auth.git

### 2. Navigate to the project folder

cd TaskManagerAuth

### 3. Restore dependencies

dotnet restore

### 4. Apply database migrations

dotnet ef database update

This will create the SQLite database used by the application.

### 5. Run the application

dotnet run

Open the address in your browser.

---

## How to Use the Application

1. Register a new account
2. Log in
3. Create tasks
4. Edit or delete tasks
5. Mark tasks as completed

Each user only sees their own tasks.

---

## Security Notes

The application includes several security measures:

- Only authenticated users can access tasks
- Users can only edit or delete their own tasks
- Anti-forgery tokens protect POST requests
- User ownership is validated against the database

---

## Future Improvements

Possible extensions for the project:

- Task categories
- Task priority levels
- Search and filtering
- API version of the application
- Deployment to a cloud platform

---

## Author

Created as a learning project while studying ASP.NET Core backend development.