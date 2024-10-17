


# Git Workflow Flowchart :

```plaintext
+---------------------+
| Working Directory    |
| (Local Changes)      |
+----------+----------+
           |
           | git add <file> or git add .
           v
+---------------------+
| Staging Area (Index)|
+----------+----------+
           |
           | git commit -m "Your commit message"
           v
+---------------------+
| Local Repository     |
+----------+----------+
           |
           | git push origin <branch>
           v
+---------------------+
| Remote Repository    |
+---------------------+
```

---

## Summary of Git Concepts

- **Working Directory**: The local folder where your project files reside. Any modifications are made here first.

- **Staging Area (Index)**: A place to prepare your changes before committing. You can selectively stage files or changes.

- **Local Repository**: A complete history of your project’s commits on your local machine. This is where changes are permanently recorded.

- **Remote Repository**: A version of your repository hosted on a server (like GitHub, GitLab, etc.), where collaboration with others happens.

---

### Example Git Workflow

1. Make changes to files in the working directory.
2. Use `git add .` to stage all the changes.
3. Commit the changes using `git commit -m "Descriptive commit message"`.
4. Push the changes to the remote repository using `git push origin <branch>`.

# Creating  a File and pushing it to Github :

## 1. File Operations Using Vim: 

### Creating and Editing Files:

- **Command**: `vim README.md`
  - Opens the `README.md` file in Vim (or creates it if it doesn't exist).
- **To Enter Insert Mode**: Press `i`
  - Allows you to start editing and adding text to the file.

### Saving and Exiting Vim:

- **To Save Changes**: Press `Esc` then type `:w`
  - Writes (saves) the changes to the file.
- **To Exit Vim**: Press `Esc` then type `:q`
  - Exits the Vim editor.
- **To Save and Exit at the Same Time**: Press `Esc` then type `:wq`
  - Saves the file and then exits.

---

## Viewing File Contents and Directory Listings

### Viewing a File’s Content:

- **Command**: `cat README.md`
- **Description**: Outputs the content of `README.md` to the terminal.

### Listing Files and Directories:

- **Command**: `ls -l`
- **Description**: Lists all files and directories in the current directory in a long format, displaying permissions, ownership, file size, and last modified date.

---

![image](https://github.com/user-attachments/assets/0e0128e0-9471-416a-917f-15d7cf87336a)

## 2.Working Directory to Staging Area:

- **Command**: `git add <file>` or `git add .`
- **Description**: Moves changes from the working directory to the staging area (index). You can add specific files or all changes.

### Staging Area to Local Repository:

- **Command**: `git commit -m "Your commit message"`
- **Description**: Commits the staged changes to the local repository with a descriptive commit message.

### Local Repository to Remote Repository:

- **Command**: `git push origin <branch>`
- **Description**: Pushes the committed changes from the local repository to the specified remote repository branch.

### Remote Repository to Local Repository:

- **Command**: `git pull origin <branch>`
- **Description**: Fetches changes from the remote repository and merges them into the current branch of the local repository.

### Checking the Status:

- **Command**: `git status`
- **Description**: Displays the current state of the working directory and staging area, showing which files are tracked, untracked, or staged.

### Viewing Commit History:

- **Command**: `git log`
- **Description**: Shows the commit history of the local repository.

---

![image](https://github.com/user-attachments/assets/56de0684-df8e-480c-9660-b26facb8076c)

