# GitHub and Git Setup for RStudio Users

## Overview

Git is a version control system that tracks changes to your files, while GitHub provides an online platform for storing, sharing, and collaborating on Git repositories. RStudio includes built-in tools that allow you to use Git without needing to work extensively in the command line.

By the end of this tutorial, you will be able to:

- Create a GitHub account
- Install Git
- Connect Git to RStudio
- Create a Git-enabled R project
- Commit changes
- Push changes to GitHub
- Pull updates from GitHub

---

# Step 1: Create a GitHub Account

1. Navigate to https://github.com
2. Click **Sign Up**
3. Choose:
   - A username
   - Email address
   - Password
4. Complete the registration process.

---

# Step 2: Install Git

Git must be installed on your computer before RStudio can use it.

### Windows

Download Git from:

https://git-scm.com/download/win

Run the installer and accept the default settings.

### Mac

Open Terminal and run:

```bash
xcode-select --install
```

or install Git through Homebrew:

```bash
brew install git
```

### Linux

```bash
sudo apt install git
```

---

# Step 3: Verify Git in RStudio

Open RStudio and select:

**Tools → Global Options → Git/SVN**

If Git is installed correctly, RStudio should automatically detect it.

If the Git executable is not found:

1. Click **Browse**
2. Locate the Git executable
3. Restart RStudio

---

# Step 4: Create a GitHub Repository

1. Go to GitHub
2. Click **New Repository**
3. Enter a repository name
4. Check **Add a README file**
5. Click **Create Repository**

Your repository is now ready to be connected to RStudio.

---

# Step 5: Clone the Repository into RStudio

Rather than creating a local repository first, the easiest workflow is to start from GitHub.

In GitHub:

1. Open your repository
2. Click the green **Code** button
3. Copy the repository URL

In RStudio:

1. Select **File → New Project**
2. Choose **Version Control**
3. Select **Git**
4. Paste the repository URL
5. Choose a local folder
6. Click **Create Project**

RStudio will automatically:

- Download (clone) the repository
- Connect it to GitHub
- Configure Git for the project

You should now see a **Git** tab in the upper-right panel.

---

# Step 6: Create a New File

Create a new R script called:

```text
hello.R
```

Add the following line:

```r
print("Hello GitHub!")
```

Save the file.

---

# Step 7: Commit Your Changes

Open the **Git** tab in RStudio.

You should see your new file listed.

1. Check the box next to `hello.R`
2. Click **Commit**
3. Enter a commit message

Example:

```text
Added hello.R script
```

4. Click **Commit**

A commit is a saved version of your project history.

---

# Step 8: Push Changes to GitHub

After committing:

1. Close the commit window
2. Click the **Push** button (green up arrow)

RStudio will upload your changes to GitHub.

Refresh the GitHub webpage and verify that your file appears online.

---

# Step 9: Pull Changes from GitHub

To practice receiving updates:

1. Open GitHub in your browser
2. Edit the README file
3. Save the changes

Back in RStudio:

1. Click the **Pull** button (blue down arrow)

The updated README file should now appear on your computer.

---

# Daily Git Workflow in RStudio

Whenever you make changes to your project:

### 1. Save your files

### 2. Stage files

Check the boxes next to modified files in the Git pane.

### 3. Commit

Click **Commit** and provide a meaningful message.

Examples:

```text
Added data analysis script
```

```text
Updated README with project description
```

```text
Fixed plotting bug
```

### 4. Push

Click **Push** to upload your changes to GitHub.

### 5. Pull

Before starting work each day (or before pushing), click **Pull** to download any changes from collaborators.

---

# Git Terms

| Term | Meaning |
|--------|---------|
| Repository | A project tracked with Git |
| Commit | A saved snapshot of changes |
| Push | Upload changes to GitHub |
| Pull | Download changes from GitHub |
| Clone | Download a repository to your computer |
| Branch | A separate line of development |

---

# Workshop Exercise

### Part 1

Create a GitHub repository called:

```text
git-workshop
```

### Part 2

Clone the repository into RStudio.

### Part 3

Create a file:

```r
practice.R
```

Add:

```r
print("My first GitHub project")
```

### Part 4

Commit the changes with the message:

```text
Initial commit
```

### Part 5

Push the changes to GitHub.

### Part 6

Edit the README file on GitHub.

### Part 7

Pull the changes into RStudio.

---

# Quick Reference

### Stage files

Use the checkboxes in the Git pane.

### Commit

Git Pane → Commit

### Push

Git Pane → Push (green up arrow)

### Pull

Git Pane → Pull (blue down arrow)

---

## Key Takeaway

**Git tracks changes on your computer, GitHub stores those changes online, and RStudio provides a user-friendly interface that allows you to work with Git and GitHub without using the command line.**
