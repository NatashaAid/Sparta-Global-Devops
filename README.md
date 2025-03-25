# Git + GitHub Cheatsheet

This is a cheatsheet I created as part of my first Git and GitHub task at Sparta Global. I started by creating my files locally in VS Code before pushing them to GitHub.

## Saving Locally First (VS Code → GitHub)

Steps I followed:

1. Create a project folder and files (e.g. `README.md`, `data.json`)
2. Open the folder in VS Code, the open terminal
3. Run `git init` to turn it into a Git repo
4. Stage your files with `git add .`
5. Commit your changes with `git commit -m "first commit"`
6. Create a GitHub repo and copy the URL
7. Link it to your local project with `git remote add origin <repo-url>`
8. Rename your branch (optional) with `git branch -M main`
9. Push to GitHub with `git push -u origin main`


## Starting on GitHub First (GitHub → VS Code)

1. Create a new repo on GitHub  
2. Copy the HTTPS clone URL  
3. `git clone <repo-url>`  
4. `cd <repo-name>`  
5. Add your files (e.g. `README.md`, `data.json`)  
6. `git add .`  
7. `git commit -m "your commit message here"`  
8. `git push`


## Common Git Commands

### Setting Up a Repo

`git init` – Create a new Git repository  
`git remote add origin <repo-url>` – Link your local repo to GitHub  
`git clone <repo-url>` – Copy a GitHub repo to your machine  

### Tracking Changes

`git status` – Check which files have been changed  
`git add <filename>` – Stage a specific file  
`git add .` – Stage all files  
`git commit -m "message"` – Commit staged changes with a message  

### Pushing to GitHub

`git push origin main` – Push local changes to the main branch  
`git pull origin main` – Pull latest changes from GitHub  

### Branching

`git branch` – View all branches  
`git checkout -b <branch-name>` – Create and switch to a new branch  
`git checkout <branch-name>` – Switch to an existing branch  
`git merge <branch-name>` – Merge another branch into the one you’re on  

### Undoing Mistakes

`git restore <filename>` – Undo changes in a file  
`git reset HEAD <file>` – Unstage a file  
`git log` – Show the commit history  