# Task Manager CLI
test2131
A simple, lightweight, and extensible command-line task manager written in Python. It helps you keep track of your tasks directly from your terminal, storing them in a local JSON file.

## Features

- **Add Tasks**: Create tasks with titles, priorities, due dates, tags, and notes.
- **List Tasks**: View all your tasks with their status and details.
- **Search Tasks**: Find tasks by keyword in their titles.
- **Manage Tasks**: Mark tasks as done, remove specific tasks, or clear all tasks.
- **Data Persistence**: Tasks are saved to `tasks.json` in the project directory.

## Installation

Ensure you have Python 3.x installed. Clone this repository and you're ready to go!

```bash
git clone <repository-url>
cd task-manager-cli
```

## Usage

### Adding a Task

Basic task:
```bash
python tasks.py add "Buy groceries"
```

Task with priority, due date, tags, and notes:
```bash
python tasks.py add "Finish project" --priority high --due "2023-12-31" --tag work --tag coding --notes "Use Python for the CLI"
```

### Listing Tasks

```bash
python tasks.py list
```

### Searching Tasks

```bash
python tasks.py search "groceries"
```

### Marking a Task as Done

```bash
python tasks.py done 1
```

### Removing a Task

```bash
python tasks.py remove 1
```

### Clearing All Tasks

```bash
python tasks.py clear
```

## Data Storage

All tasks are stored in a `tasks.json` file in the same directory as `tasks.py`. This file is automatically created when you add your first task.
