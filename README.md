````markdown
# Git & VS Code Setup Guide for Azubis at HYDAC (Windows)

Welcome!  
In this exercise, you will prepare your computer for working with Git, GitHub, Visual Studio Code, and the Windows terminal.

This guide is written for complete beginners.  
Please follow the steps slowly and in order.

---

## Goal of this first part

At the end of this setup, you should have:

- a GitHub account
- Git installed
- Visual Studio Code installed
- a terminal you can use
- your repository cloned to your computer
- a basic understanding of a few terminal commands

This first part is only about **installation and preparation**.  
We will continue with branches, commits, and feature development afterwards.

---

## Time estimate

Take your time.  
This part can be done slowly in about **2 to 3 hours**, even if you are completely new.

---

## What you need

Before you start, make sure you have:

- a Windows computer
- internet access
- permission to install software
- a GitHub account

If you do not yet have a GitHub account, create one first.

---

# 1. Install Git

## What is Git?

Git is a tool that helps programmers track changes in files.  
It is used in almost every software project.

## What to install

Install **Git for Windows**.

During installation, the default options are fine for this exercise.

## Important check after installation

After installation:

1. Open the **Command Prompt** or **PowerShell**
2. Type:

```bash
git --version
````

3. Press **Enter**

If Git is installed correctly, you should see something similar to:

```bash
git version 2.x.x.windows.x
```

If you see a version number, Git is ready.

---

# 2. Install Visual Studio Code

## What is VS Code?

Visual Studio Code (VS Code) is a code editor.
You will use it to view and edit files in the repository.

## What to do

Install **Visual Studio Code**.

During installation, it is helpful if you enable these options:

* **Add "Open with Code"**
* **Add to PATH**
* **Register Code as editor for supported file types**

If you are unsure, ask for help during installation.

## Important check after installation

Open VS Code.

If it starts normally, the installation worked.

---

# 3. Open a terminal on Windows

You will use the terminal to type commands.

A terminal is simply a text-based way to talk to your computer.

## Which terminal can you use?

For this exercise, you can use one of these:

* **PowerShell**
* **Command Prompt**
* **Terminal in VS Code**

For beginners, the easiest option is often:

* open **VS Code**
* then open the terminal inside VS Code

## How to open the terminal in VS Code

1. Open VS Code
2. Click **Terminal**
3. Click **New Terminal**

A terminal window should open at the bottom.

---

# 4. Learn a few important terminal basics

Do not worry about memorizing everything.
You only need a few commands at the start.

---

## 4.1 What is a command?

A command is text you type into the terminal.
Then you press **Enter** to run it.

Example:

```bash
git --version
```

---

## 4.2 Where am I right now?

To see your current folder, type:

```bash
pwd
```

In PowerShell, this shows your current path.

Example:

```bash
C:\Users\YourName
```

---

## 4.3 Show files and folders

To see what is inside the current folder, type:

```bash
dir
```

This shows files and folders.

---

## 4.4 Change into another folder

To move into a folder, use:

```bash
cd foldername
```

Example:

```bash
cd Desktop
```

This changes into your Desktop folder.

To go one folder back, use:

```bash
cd ..
```

---

## 4.5 Create a new folder

To create a folder, use:

```bash
mkdir foldername
```

Example:

```bash
mkdir projects
```

---

## 4.6 Clear the terminal

If the terminal becomes messy, type:

```bash
clear
```

If that does not work, try:

```bash
cls
```

---

# 5. Create a folder for your programming projects

It is a good idea to keep your work in one place.

## Step

In the terminal, go to your user folder first:

```bash
cd C:\Users\YourName
```

Replace `YourName` with your Windows username.

Now create a projects folder:

```bash
mkdir projects
```

Go into it:

```bash
cd projects
```

Check where you are:

```bash
pwd
```

You should now be inside your `projects` folder.

---

# 6. Configure Git for the first time

Git should know your name and email address.

Use the same email address that you use for GitHub.

## Commands

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Example:

```bash
git config --global user.name "Max Mustermann"
git config --global user.email "max.mustermann@example.com"
```

## Check your settings

```bash
git config --global --list
```

You should see your name and email.

---

# 7. Sign in to GitHub

Make sure you can log in to your GitHub account in the browser.

You will need:

* your GitHub username
* your password
* possibly two-factor authentication if enabled

---

# 8. Get the repository URL

Your trainer will provide you with the repository URL.

It will look similar to this:

```bash
https://github.com/ORG-NAME/REPOSITORY-NAME.git
```

Example:

```bash
https://github.com/example-company/git-training.git
```

Do not invent the URL yourself.
Use the exact one that is given to you.

---

# 9. Clone the repository

## What does "clone" mean?

To clone a repository means:

* copy it from GitHub
* download it to your computer
* connect your local copy to the remote repository

## Step-by-step

Make sure you are still inside your `projects` folder.

Then type:

```bash
git clone REPOSITORY-URL
```

Example:

```bash
git clone https://github.com/example-company/git-training.git
```

Press **Enter**.

If everything works, Git will create a new folder with the repository name.

---

# 10. Go into the repository folder

After cloning, enter the new folder.

Example:

```bash
cd git-training
```

Now check what is inside:

```bash
dir
```

---

# 11. Open the repository in VS Code

When you are inside the repository folder in the terminal, type:

```bash
code .
```

This opens the current folder in VS Code.

## If `code .` does not work

If you get an error, open VS Code manually:

1. Start VS Code
2. Click **File**
3. Click **Open Folder**
4. Select your repository folder

---

# 12. Check the Git status

Inside the repository folder, type:

```bash
git status
```

This command is very important.

It shows:

* which branch you are on
* whether files were changed
* whether something is ready to commit

At the beginning, it should usually say that nothing has changed.

---

# 13. Understand the folder structure

Once the repository is open in VS Code:

1. Look at the files on the left side
2. Open the `README.md` file if there is one
3. Do not change anything yet unless you are told to

The goal here is only to become familiar with the project.

---

# 14. Very important beginner rules

Please follow these rules:

* Work slowly
* Read each command before pressing **Enter**
* Copy commands carefully
* If you get an error, read it calmly
* Do not panic if something does not work immediately
* Ask questions when needed
* Do not randomly delete files
* Do not randomly click Git buttons in VS Code if you do not understand them yet

---

# 15. Common commands you should know already

Here is a short overview:

## Show current folder

```bash
pwd
```

## Show files in current folder

```bash
dir
```

## Change folder

```bash
cd foldername
```

## Go one folder back

```bash
cd ..
```

## Create folder

```bash
mkdir foldername
```

## Check Git version

```bash
git --version
```

## Check Git status

```bash
git status
```

## Clone repository

```bash
git clone REPOSITORY-URL
```

## Open current folder in VS Code

```bash
code .
```

---

# 16. What to do if something does not work

## Git command not found

Possible reason: Git was not installed correctly.

Try:

* closing and reopening the terminal
* restarting the computer
* reinstalling Git

---

## `code .` does not work

Possible reason: VS Code was not added to PATH.

Use VS Code manually with **File > Open Folder**.

---

## Permission error during installation

Possible reason: You need admin rights.

Ask your trainer or IT support.

---

## GitHub login problems

Check:

* username
* password
* internet connection
* two-factor authentication

---

# 17. Checklist

Before continuing to the next exercise, make sure all of these are done:

* [ ] GitHub account exists
* [ ] Git is installed
* [ ] `git --version` works
* [ ] VS Code is installed
* [ ] Terminal can be opened
* [ ] A `projects` folder exists on the computer
* [ ] The repository was cloned
* [ ] The repository folder can be opened in VS Code
* [ ] `git status` works inside the repository

---

# 18. Stop here for now

If you have completed all steps above, you are ready for the next part.

In the next part, we will learn how to:

* create your own branch
* make changes
* save them with commits
* push them to GitHub

Do not continue with branches or commits yet unless instructed to do so.

---

# 19. Optional practice

If you finish early, practice these commands a few times:

```bash
pwd
dir
cd ..
cd projects
git status
```

The goal is simple:
feel comfortable opening the terminal, moving through folders, and checking Git status.

---

# 20. Final note

Nobody starts as an expert.
If this is your first time using Git, GitHub, VS Code, or a terminal, that is completely fine.

The important thing is:

* follow the steps carefully
* stay calm
* learn one command at a time

```

If you want, I can now turn this into a **more polished company-internal README** with HYDAC wording and placeholders for your exact repo name.
```
