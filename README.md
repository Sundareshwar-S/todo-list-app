# 📝 Todo List App (Flask + SQLite)

A clean and simple Todo List app built with **Flask** and **SQLite**, styled with custom CSS. This app supports basic CRUD operations — add, complete, and delete tasks — with data stored in a local SQLite database.

🌐 **Live Demo:**  
👉 [https://shine-chalk-bovid.glitch.me](https://shine-chalk-bovid.glitch.me)

---

## ✨ Features

- ✅ Add new tasks with a title and optional description
- ✅ Toggle task completion (with a satisfying strikethrough)
- ✅ Delete tasks with one click
- ✅ Persistent storage using **SQLite**
- 🎨 Responsive UI with clean CSS styling
---

## 📁 Project Structure
---
todo-list-app/ 
├── app.py # Main Flask application 
├── requirements.txt # Python dependencies 
├── start.sh # Glitch startup script 
├── .glitch.json # Glitch configuration 
├── templates/ 
│ └── index.html # HTML template (Jinja2) 
└── static/ 
└── style.css # CSS styling
---
## 🧠 Tech Stack

- **Backend**: Flask (Python)
- **Database**: SQLite (with SQLAlchemy)
- **Frontend**: HTML + CSS (Jinja2 templates)
---
## How It Works

1. **Homepage (`/`)**:
   - Displays a list of tasks stored in the SQLite database.
   - Each task shows its title, description, and completion status.
   - Provides options to mark tasks as completed or delete them.

2. **Add Task (`/add`)**:
   - Users can add a new task by submitting a form with a title (required) and an optional description.
   - The task is saved in the database and displayed on the homepage.

3. **Mark Task as Completed (`/complete/<id>`)**:
   - Toggles the completion status of a task.
   - Clicking the ✅ icon marks a task as completed or uncompleted.

4. **Delete Task (`/delete/<id>`)**:
   - Deletes a task from the database.
   - Clicking the 🗑️ icon removes the task permanently.

5. **Database**:
   - Uses SQLite to store tasks.
   - The `Task` model includes fields for `id`, `title`, `description`, and `completed` status.

6. **Frontend**:
   - The UI is built using an HTML template (`index.html`) styled with CSS (`style.css`).
   - Tasks are dynamically rendered using Jinja2 templating.

7. **Backend**:
   - Built with Flask.
   - Routes handle user interactions and database operations.

8. **Hosting on Glitch**:
   - The app is hosted on [Glitch.com](https://glitch.com).
   - Glitch automatically installs dependencies from `requirements.txt` and runs the app using the `start.sh` script.
   - The app listens on `0.0.0.0` and uses the `PORT` environment variable provided by Glitch.
   ---
