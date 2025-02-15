# Git and GitHub Guide

## Installation

1. Open browser: [Git Download Page](https://git-scm.com/downloads)
2. Download Git
3. Open the downloaded Git installer
4. Follow the setup instructions to install Git

## Commands to Check Git Version and Configuration
git --version
git config
git config --global --list


## Setup Global Configuration
git config --global user.name "name"
git config --global user.email "email_id"

## Repository Initialization and Branch Setup
# Initialize the repository with the 'main' branch
git init -b main

# Rename the 'main' branch to 'master'
git branch -m main master

# Delete the 'main' branch on the remote
git push origin --delete main

# Push the 'master' branch and set the upstream
git push -u origin master

## First Project
```sh 
  # Create Local Repo
    git status
    git init
    git init -b main
  
  # Commit Changes
    git add filename.txt
    git log
    git commit -m "message/changes what you have done..."
    git log

  # Git Staging and Skipping Area
    git status
    git add filename.txt
    git commit -m "second commit"
    git log
    git commit -a -m "third commit"

  # Git Remove
    git add .
    git status
    git commit -m "added all project"
    git status
    git rm --cached filename
    git status
    git commit -m "removed the unwanted files"

## Connenting to GitHub Repository
  git init
  git remote add origin git@github.com:your_username/my-project-repo.git
  git remote -v
  git add .
  git branch
  git checkout -b main
  git add .
  git commit -m "Initial commit"
  cat ~/.ssh/id_ed25519.pub
  ssh -T git@github.com
  git remote add origin git@github.com:your_username/my-project-repo.git
  git push -u origin main
  git log


