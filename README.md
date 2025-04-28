# 📋 Advanced CLI Task Manager

A simple command-line task manager built with Python.  
It uses `argparse`, **subcommands**, **environment variables**, **logging**, and includes **unit tests**.

---

## 🚀 Features

- Add a task with a description and priority
- List all tasks
- Delete a task by ID
- Tasks are stored in a `JSON` file
- All actions are logged to a log file
- Task file path can be configured through an environment variable
- Includes unit tests for core features

---

## 📦 Project Structure

```plaintext
advanced_cli_task_manager/
├── README.md
├── requirements.txt
├── task_manager/
│   ├── __init__.py
│   ├── cli.py
│   ├── config.py
│   ├── core.py
│   └── logger.py
├── tasks.json
└── tests/
    └── test_core.py
```

---

## 🔧 Installation

1. Clone the repository:

```bash
git clone <repository_url>
cd advanced_cli_task_manager
```

2. Install the dependencies:

```bash
pip3 install -r requirements.txt
```

(Use `pip3` if you are on macOS.)

---

## 💪 Usage

**Add a Task:**
```bash
python3 -m task_manager.cli add "Do the homework" 2
```

**List Tasks:**
```bash
python3 -m task_manager.cli list
```

**Delete a Task:**
```bash
python3 -m task_manager.cli delete 1
```

---

## 🛠️ Configuration

You can specify a custom tasks file by setting the `TASKS_FILE_PATH` environment variable.

**Example:**
```bash
export TASKS_FILE_PATH="/path/to/your/tasks.json"
```

---

## 📊 Running Tests

Run the unit tests with:

```bash
pytest
```

(Make sure you are in the project root directory.)

---
