
# 📝 Dockerized To-Do List App

This project is a simple two-tier web application—a to-do list—that demonstrates Docker Compose in action. It was built as part of a Docker workshop and is a great example of containerizing multi-service applications.

## 📦 Project Structure

```
.
├── docker-compose.yml
├── app/                 # Frontend/Backend app source code
└── db/                  # Database initialization scripts (if any)
```

## 🧱 Tech Stack

- **Frontend + Backend**: React and 
- **Database**: MySQL
- **Docker Compose**: For orchestrating services

## 🚀 How to Run

1. **Clone this repo**

```bash
git clone https://github.com/yourusername/docker-todo-app.git
cd docker-todo-app
```

2. **Start the app**

```bash
docker-compose up --build
```

3. Visit the app in your browser:

```
http://localhost:3000
```

> Port might differ depending on your setup.

## 🛠 Features

- Add, delete, and complete tasks
- Persistent storage using a database container
- Docker Compose-managed networking
- Easy local development and teardown

## 🐳 Docker Highlights

- Multi-container orchestration via `compose.yaml`
- Named volumes for persistent data
- Service dependencies (app waits for DB to be ready)

## 📂 Environment Variables

You can configure settings via a `.env` file (if supported):

```env
DB_HOST=db
DB_USER=todo_user
DB_PASSWORD=secret
DB_NAME=todo_app
```


This project was inspired by the official Docker Workshop. Big thanks to the maintainers and contributors!

