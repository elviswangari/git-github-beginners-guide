# Introduction to Git and GitHub for beginners

## Learning Objectives:
1. Understand what Git and GitHub are and their importance.
2. Learn basic Git commands to manage versions locally.
3. Learn how to clone an existing repository from GitHub.
4. Learn how to create a repository from an existing project locally.
5. Know how to push and pull changes to GitHub.
6. Complete basic tasks like initializing a repository, committing changes, and collaborating via GitHub.

---

## 1. Introduction to Git and GitHub

### What is Git?
- Git is a version control system that helps track changes in code.
- Think of Git as a way to save "checkpoints" in your project.
- It allows multiple people to collaborate on projects without losing track of changes.
- Git is a tool to track changes in files over time.
- Think of Git as a way to save "checkpoints" in your project.

### What is GitHub?
- GitHub is a cloud-based platform that hosts Git repositories.
- It allows you to store, manage, and collaborate on Git projects online.
- GitHub is a cloud platform where you can store your Git projects online.
- It makes it easy to collaborate with others and keep your code safe.

### Why Use Git and GitHub?
- Manage code versions.
- Collaborate efficiently with team members.
- Keep a backup of your projects.

---

## 2. Two Ways to Start a Git Project
(a) Cloning an Online Repository  
(b) Creating a Local Repository and Pushing it to GitHub

---

## 2. Two Ways to Start a Git Project
(a) Cloning an Online Repository  
(b) Creating a Local Repository and Pushing it to GitHub

---

## 3. Practical Part 1: Cloning an Existing Repository

### Scenario: Download (clone) an existing project from GitHub and make some changes.

1. **Create a repository on GitHub**:
    - Go to GitHub, click New Repository.
    - Name it `my-cloned-repo`, leave it empty for now (no files), and click Create.

2. **Copy the repository URL**:
    - On the repo page, click the green Code button and copy the URL.

3. **Clone the repository to your computer**:
    - Open Terminal/Command Prompt and type:
      ```bash
      git clone <GitHub-Repository-URL>
      ```
    - This will create a folder with the name of the repository.

4. **Navigate to the cloned repository**:
    ```bash
    cd my-cloned-repo
    ```

5. **Create a new file (example: hello.txt)**:
    ```bash
    echo "Hello from the cloned repo!" > hello.txt
    ```

6. **Stage and commit the file**:
    - Stage the file:
      ```bash
      git add hello.txt
      ```
    - Commit the changes:
      ```bash
      git commit -m "Add hello.txt"
      ```

7. **Push the changes back to GitHub**:
    ```bash
    git push origin main
    ```

8. **Check GitHub**: You’ll see your new file online in your repo.

---

## 4. Practical Part 2: Creating a Local Repository with `git init` (10 minutes)

1. **Create a new folder on your computer**:
    - Name it `git_project` and navigate into it using the terminal:
      ```bash
      mkdir git_project 
      cd git_project
      ```

2. **Initialize Git in the folder**:
    ```bash
    git init
    ```
    - This tells Git to start tracking changes in this folder.

3. **Create a new file (example: readme.txt)**:
    ```bash
    echo "This is a local repo." > readme.txt
    ```

4. **Stage and commit the file**:
    - Stage the file:
      ```bash
      git add readme.txt
      ```
    - Commit the changes:
      ```bash
      git commit -m "Add readme.txt"
      ```

5. **Create a new repository on GitHub**:
    - Go to GitHub, click New Repository.
    - Name it `github_project` and create it.

6. **Connect your local repo to GitHub**:
    - In your terminal, link the local repo to the GitHub repo:
      ```bash
      git remote add origin <GitHub-Repository-URL>
      ```

7. **Push your changes to GitHub**:
    ```bash
    git push -u origin main
    ```

8. **Check GitHub**: Your local files will be uploaded.

---

## 5. Practical Recap and Q&A
