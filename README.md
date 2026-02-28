# ✅ GoCheck — Task Management System

> A Java-based goal and task management application built using the Stack data structure (LIFO), designed to help users organize their goals and break them down into achievable daily tasks.

---

## 📖 About the Project

**GoCheck** is a console-based Java application developed as a course project for *CS310: Data Structures* at Imam Abdulrahman Bin Faisal University. The system allows users to manage their personal goals across seven life aspects — Career, Spirituality, Physical Health, Personal Growth, Relationships, Finances, and Entertainment — by organizing them into stacks and breaking them down into actionable tasks.

The program implements a **Stack data structure** using a **linked list**, following the Last-In-First-Out (LIFO) principle for efficient memory usage and task management.

---

## 🚀 Features

### 👤 User Role
- **Account System** — Register or log in with unique username, email, and phone number validation
- **Choose from Suggestions** — Browse 35 pre-defined goals (5 per life aspect) loaded from a file, and auto-generate associated tasks with suggested due dates
- **Create Your List** — Build a fully custom goal and task list with priority and due date settings
- **Manage Your List:**
  - Add new tasks (from suggestions or custom)
  - Update goal text, task description, priority, aspect, or due date
  - Check off (pop) goals/tasks: top, at position, or all at once
  - Display goals and tasks stack
  - Sort by due date (ascending/descending) or by priority (high/low)
  - Search tasks by due date

### 🔐 Admin Role
- Pre-defined admin accounts (not user-creatable)
- **Create Suggestion Templates** — Add new goal templates with tasks and suggested due dates across any life aspect
- **Manage Created Lists** — Add, update, and display admin-created task lists
- **Print Report** — Generate an activity report file showing number of add, delete, update, and display operations performed

---

## 🏗️ System Architecture

The project is built around **10 core classes:**

| Class | Description |
|---|---|
| `GoCheck` | Main entry point; handles user/admin menus |
| `User` | All user operations (suggestions, custom lists, manage) |
| `Admin` | All admin operations (templates, manage, reports) |
| `Account` | Linked list of user/admin accounts with validation |
| `Task` | Task object with text, priority, aspect, and due date |
| `Goal` | Goal object with text, priority, aspect, and due date |
| `TaskStack` | Stack of tasks (linked list) with full CRUD + sort |
| `GoalsStack` | Stack of goals (linked list) with full CRUD + sort |
| `AdminTaskStack` | Admin-only version of TaskStack |
| `AdminGoalsStack` | Admin-only version of GoalsStack |

---

## 🎯 Goal Aspects Supported

1. 💼 Career
2. 🕌 Spirituality
3. 💪 Physical Health
4. 🌱 Personal Growth
5. 🤝 Relationships
6. 💰 Finances
7. 🎭 Entertainment

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Java** | Core application logic and data structures |
| **Java Swing (JOptionPane)** | GUI dialogs for input/output |
| **LinkedList (custom)** | Stack implementation |
| **LocalDateTime** | Task and goal due date management |
| **File I/O** | Reading suggestion lists and writing admin reports |
| **NetBeans IDE** | Development environment |

---

## ⚙️ Setup & Installation

### Prerequisites
- Java JDK 8 or higher
- NetBeans IDE (recommended) or any Java IDE

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/norahalanziii/GoCheck.git
   cd GoCheck
   ```

2. **Open in NetBeans**
   Open the project folder as an existing NetBeans project

3. **Run the project**
   Run `GoCheck.java` as the main class


---

## 🎮 How It Works

```
Launch GoCheck
│
├── 1. User
│   ├── Log In / Sign Up
│   └── Main Menu
│       ├── Choose from Suggestions  → Pick goal → Auto-generate tasks
│       ├── Create Your List         → Custom goal + tasks
│       └── Manage Your List
│           ├── Add / Update Tasks
│           ├── Check (pop) Goals & Tasks
│           ├── Display Lists
│           └── Sort Tasks
│
└── 2. Admin
    ├── Log In (pre-defined accounts only)
    └── Admin Menu
        ├── Create Suggestion Templates
        ├── Manage Created Lists
        └── Print Activity Report → saved to file
```
---

---

## 📄 License

This project was developed for academic purposes as part of the CS310 Data Structures course project, Academic Year 2023/2024.
