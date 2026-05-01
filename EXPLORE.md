# Explore git 4
$ git config --global user.name "tejat2231-1gtm"
$ git config --global user.email "tejat2231@gmail.com"
$ git init
$ git status On branch master
$ git add
$ git commit - "Initial commit"
$ git remote add origin https://github.com/tejat2231-1gtm/shoping.git
$ git commit -m "first commit"
$ git push-u origin main

# Create Repo + README + Push 5

mkdir myrepos
$ cd myrepos 
 $ git init
$ echo "# My college" > README.md
$ git add README.md
 $ git commit -m "Added README file" 
$ git remote add origin https://github.com/tejat2231-1gtm/boys.git
$ git branch -M main
 $ git push-u origin main

 # Create Branch & Merge 6

$ git branch MITS
$ git checkout MITS
$ echo "Branch work" >> file.txt
$ git add . 
git commit -m "changes in MITS branch"
$ git checkout main
$ git merge MITS


# View Commit History 7

$ mkdir exp7
$ cd exp7
$ git init 
$ echo "First version" >file.txt
$ git add file.txt
$ git config --global user.gmail"tejat2231@gmail.com"
 $ echo "First version">>file.txt
$ git commit -n "first commit"
$ git log

# Clone Repository 8
git clone https://github.com/username/repo.git
 
 # Push Changes to Remote  9

$ echo "New changes" >> file.txt

$ git add.

$ git commit -m "Updated file"

5 git push

 # Scrum / Kanban Board 2 
 Done directly in GitHub
Steps:
Go to your repository
Click Projects
Click New Project
Select Board (Kanban)
Create columns:
To Do
In Progress
Done
Add tasks (cards)
Move tasks between columns

# Continuous Testing (Simple) 3
$ git init 
$ git status
 $ git add tejaswini.txt

 $ git config --global user.name "tejat2231-1gtm"

 $ git config --global user.email "tejat2231@gmail.com"

$ git commit -m "first commit"
 $ git remote add origin https://github.com/tejat2231-1gtm/tik-tok.git

 $ git branch -M main
$ git push-u origin main


# Continuous Integration (CI) 1

Step-by-Step Process
🔹 Step 1: Create project in your system
Bash
mkdir ci-project
cd ci-project
git init
🔹 Step 2: Create a simple file
Bash
echo "print('Hello CI')" > app.py
🔹 Step 3: Add & commit
Bash
git add .
git commit -m "Initial commit"
🔹 Step 4: Connect to GitHub
Bash
git remote add origin https://github.com/YOUR-USERNAME/ci-project.git
git branch -M main
git push -u origin main
🔹 Step 5: Create CI file in GitHub
👉 Inside your project folder create:
📁 .github/workflows/
📄 ci.yml
🔹 Step 6: Add this code in ci.yml
YAML
name: CI Pipeline

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v3

    - name: Setup Python
      uses: actions/setup-python@v4
      with:
        python-version: '3.x'

    - name: Run Program
      run: python app.py
🔹 Step 7: Push again
Bash
git add .
git commit -m "Added CI file"
git push

