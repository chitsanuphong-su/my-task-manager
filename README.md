
# My Simple Task Manager CLI

A lightweight, interactive Command-Line Interface (CLI) application built with Python to manage daily tasks efficiently. All task data is automatically persisted using JSON format.

## Features

* **Add Tasks**: Add new tasks with descriptions and automatically assigned unique IDs.
* **List Tasks**: View all recorded tasks along with their ID, description, and status (Pending / Completed).
* **Complete Tasks**: Mark specific tasks as completed by entering their Task ID.
* **Delete Tasks**: Safely remove unwanted tasks by their Task ID.
* **Data Persistence**: Tasks are saved to `data/tasks.json` upon exit and loaded automatically on startup.
* **Robust Error Handling**: Handles invalid menu selections, non-numeric inputs, and missing/corrupted data files without crashing.

## Project Structure

```text
my-task-manager/
├── src/
│   ├── __init__.py      # Marks 'src' directory as a Python package
│   ├── task_data.py     # Handles reading and writing tasks to JSON
│   └── task_logic.py    # Implements core task management operations
├── data/
│   └── tasks.json       # Stores task data (created automatically)
├── main.py              # Main application entry point and user interaction loop
├── .gitignore           # Specifies untracked files for Git to ignore
└── README.md            # Project documentation

```

## Prerequisites

* **Python**: Version 3.7 or higher installed on your system.
* **Git**: Installed for version control.

## Installation & Setup

1. **Clone the Repository:**
```bash
git clone [https://github.com/YOUR_USERNAME/my-task-manager.git](https://github.com/YOUR_USERNAME/my-task-manager.git)
cd my-task-manager

```


2. **Set Up Virtual Environment (Optional but Recommended):**
* **Windows (CMD):**
```cmd
python -m venv venv
venv\Scripts\activate

```


* **macOS / Linux:**
```bash
python3 -m venv venv
source venv/bin/activate

```




3. **Run the Application:**
```bash
python main.py

```



## How to Use

When you run `main.py`, you will see an interactive menu:

```text
--- Task Manager Menu ---
1. Add Task
2. List Tasks
3. Complete Task
4. Delete Task
5. Exit
-------------------------
Enter your choice (1-5): 1
Enter task description: Finish Python Lab Week 7
Task 'Finish Python Lab Week 7' added with ID 1.

```

Follow the on-screen prompts by entering numbers `1` through `5` to perform actions.

## License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).

```

```