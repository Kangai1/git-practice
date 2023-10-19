# Git and Shell Commands Guide

## Git Configuration Levels

Git configurations are stored at three levels:

1. **System Level:** These settings affect the entire system and require administrative privileges.
   - File Location: `/etc/gitconfig`

2. **Global (User) Level:** User-specific settings that affect all repositories of the current user.
   - File Location: `~/.config/git/config`

3. **Local Level:** These settings are specific to the current repository.
   - File Location: `.git/gitconfig`

Each level can override values in the previous level, with the following priority: System Level -> Global Level -> Local Level.

## Basic Git Commands

- git init
- git status
- git add [file_name]
- git add .
- git rm --cached [file_name]
- git commit -m "commit message"
- git log

# Basic Git explanation

1. **Initialize a Git Repository**
   - Initialize a Git repository with the command `git init`.

2. **Check the Status**
   - Before committing changes, it's a good practice to check the status of your files.
   - Use the `git status` command to do so.

3. **Stage Files for Commit**
   - Staging is the process of preparing files for a commit.
   - Stage a specific file for the next commit: `git add [file_name]`
   - Stage all changes for the next commit: `git add .`

4. **Unstage Files**
   - If you accidentally stage a file or want to unstage a file that was previously staged, you can use the following command:
   - `git reset [file_name]`.

5. **Commit Changes**
   - Once you have staged the changes you want to include in the next commit, you can commit those changes with a commit message:
   - `git commit -m "commit message"`

6. **View Commit History**
   - To view the commit history, you can use the `git log` command. This will display a list of commits along with their details.
   - `git log`

These are the fundamental steps for managing your files and tracking changes in your Git repository. Using these commands, you can effectively maintain your project's history.
