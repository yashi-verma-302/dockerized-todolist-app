Dockerized ToDo List Application

A simple ToDo List application containerized with Docker. This application allows users to add, view, and delete tasks. It can be easily deployed on any system with Docker installed.

Prerequisites

Docker: Download and Install Docker
Docker Compose (optional): Download and Install Docker Compose

Getting Started
Clone the repository:

Go to your terminal:
git clone https://github.com/yourusername/todolist-app.git
cd todolist-app
Build the Docker image:

bash
Copy code
docker build -t todolist-app .
Run the application:

bash
Copy code
docker run -p 5000:5000 todolist-app
The application should now be accessible at http://localhost:5000.

Using Docker Compose (Optional)
If a docker-compose.yml file is included, you can build and run the application with Docker Compose:

bash
Copy code
docker-compose up
Features
Add Tasks: Create a new to-do item.
View Tasks: See a list of all current tasks.
Delete Tasks: Remove tasks when completed.
Environment Variables
Variable	Description	Default
PORT	Application port	5000
DATABASE	Database file or URL	sqlite:///tasks.db
Built With
Python and Flask for the backend.
SQLite for task storage.
