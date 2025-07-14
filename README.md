# cintel-04-local

## **How to Install and Run a Project**
---
### **Step 1. Create a New Repo in GitHub**
 - Open your browser and log in to your GitHub account.
 - Select 'Create New Repository' from the dropdown menu, and name your repo.
 - Select the Public option so others can view your repository, and add a README.md file.
 - Click the 'Create repository' button to finalize the process.
 - Clone your repo to local using your new URL pasted into the following example command.
  - git clone https://github.com/youraccount/yourrepo
 - Create your .gitignore and requirements.txt files.
 - Run the following command from your project route directory to create your virtual environment.
  - py -m venv .venv
 - Use the following commands to add files to version control.
IMPORTANT: Replace the commit message with a clear and descriptive note about what you added or changed.
  - git add .    # stages changes, adds files to source control
  - git commit -m "Add .gitignore and requirements.txt files"    # creates a labeled snapshot of staged changes.
  - git push -u origin main    # updates the remote repository
 - Open the newly cloned folder to begin working in it by selecting 'file' 'open folder' navigate to the new repo and select 'open'.
---
### **Step 2. Activate Your .venv**
 - Before making any changes to a project, ALWAYS pull the latest changes from the remote repository on GitHub using the following command.
  - git pull origin main
 - Run the following command to activate your .venv # HINT- You MUST activate your .venv before editing a project.
  - .venv\Scripts\activate
---
### **Step 3. Install Packages Into Your Local Project Virtual Environment**
 - Ensure your .venv is active, update key packages, and install dependencies from your requirements.txt using the following commands.
  - .venv\Scripts\activate
  - py -m pip install --upgrade pip setuptools wheel
  - py -m pip install -r requirements.txt
---
## **Repeatable Project Workflow**
 Follow these steps when starting a new work session on a professional Python project.
### **1. Pull the Latest Changes from GitHub:**
  - git pull origin main
### **2. Activate the Project Virtual Environment:**
  - .venv\Scripts\activate
### **3. Install Dependencies As Needed:**
  - py -m pip install -r requirements.txt
### **4. Run Scripts as needed:**
  - select python interpreter for your local venv
  - py myfile.py   
### **5. Run Jupyter Notebooks as needed:**
 - click the kernel selector in the top-right corner of the notebook editor and choose the interpreter associated with your .venv.
 - Click on a cell and press Shift+Enter to execute it and move to the next cell.
 - Alternatively, use Ctrl+Enter to execute the current cell without moving.
 - Use 'Run ALL' to execute notebooks fully before running git add-commit-push to GitHub.
 - Save your notebook periodically to avoid losing progress. Or make sure the File / Autosave option is on.
### **6. Save your work with git add-commit-push to GitHub:**
  - git add .    
  - git commit -m "Add your unique message here." 
  - git push -u origin main  