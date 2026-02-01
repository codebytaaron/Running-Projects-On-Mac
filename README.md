# Running the Project (macOS)

This guide explains how to start the backend and frontend locally using the macOS Terminal.

---

## Prerequisites

- macOS
- Python 3 installed (`python3 --version` to check)
- Terminal
- Web browser

---

## Start the Backend (Python)

1. Open **Terminal**

2. Navigate to the backend folder:
```bash
cd ~/Desktop/URL-Status-Checker/backend
Create a virtual environment:

python3 -m venv .venv
Activate the virtual environment:

source .venv/bin/activate
Install dependencies:

pip install -r requirements.txt
Start the backend server:

uvicorn main:app --reload
If successful, the backend will run at:

http://127.0.0.1:8000
Leave this terminal window open.

Start the Frontend (New Terminal Window)
Open a new Terminal window

Navigate to the frontend folder:

cd ~/Desktop/URL-Status-Checker/frontend
Start a local web server:

python3 -m http.server 5500
The frontend will be available at:

http://localhost:5500
Leave this terminal window open.

Stopping the Servers
To stop either server:

Click the terminal window

Press Control + C

Notes
The backend and frontend must be running at the same time

If a port is already in use, change 5500 to another number (for example 5501)

If python does not work, always use python3

