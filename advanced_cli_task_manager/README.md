# Advanced CLI Task Manager

This project is a CLI-based Task Manager with subcommands, logging, environment variables, and testing.

## Requirements

- Python 3.x
- `argparse` (part of the Python standard library)
- `unittest` (part of the Python standard library)

## Setup

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Lthath/python-in-devops
    cd advanced_cli_task_manager
    ```

2. **Create and activate a virtual environment**:
    - On macOS and Linux:
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
    - On Windows:
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Running the CLI Tool

Before running the CLI tool, set the `PYTHONPATH` environment variable to include the parent directory of the `task_manager` package:

```bash
export PYTHONPATH=$(pwd)
```

```bash

# Add a Task

python task_manager/cli.py add "Test Task" 1

# List Tasks

python task_manager/cli.py list

# Delete a Task

python task_manager/cli.py delete 1

# Running Tests

python -m unittest discover -s tests

# Testing the Logger

python tests/test_logger.py

```