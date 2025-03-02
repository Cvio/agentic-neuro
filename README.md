## Setup Guide

Welcome to this repository! Follow these steps to clone the repo, set up a virtual environment, and install dependencies to get started quickly.


## Clone the Repository
First, download the project to your local machine:
```bash
# Using HTTPS
git clone https://github.com/Cvio/agentic-neuro.git

# Using SSH
git clone git@github.com:Cvio/agentic-neuro.git
```

Change into the project directory:
```bash
cd agentic-neuro
```


## Create and Activate a Virtual Environment
To ensure dependencies remain isolated, create a virtual environment:

### **Mac/Linux**
```bash
python3 -m venv venv
source venv/bin/activate
```

### **Windows (Command Prompt)**
```cmd
python -m venv venv
venv\Scripts\activate
```

### **Windows (PowerShell)**
```powershell
python -m venv venv
venv\Scripts\Activate
```

## Install Dependencies
With the virtual environment active, install the necessary packages:
```bash
pip install -r requirements.txt
```

If you add new dependencies, remember to update `requirements.txt`:
```bash
pip freeze > requirements.txt
```

## Deactivating the Virtual Environment
When finished, deactivate the virtual environment:
```bash
deactivate
```


## Ignoring the Virtual Environment in Git
To keep your repository clean, ensure `venv/` is ignored by Git:
```bash
echo "venv/" >> .gitignore
git rm -r --cached venv/
```


## Next Steps
- If you run into issues, ensure your Python version is correct (`python --version`).
- If a package is missing, check `requirements.txt` and reinstall with `pip install -r requirements.txt`.
- Need help? Create an issue in this repository!
