# Documentation for Forking and Working on a GitHub Project

## Purpose

This document provides an overview of the steps I followed to fork a GitHub repository, work on the project locally, and update it in my personal GitHub account.

---

## Steps Followed

### 1. Forking the Repository
1. **Navigated to the repository page**: Selected the repository I wanted to fork.
2. **Clicked the "Fork" button**: Created a complete copy of the repository under my personal GitHub account.
3. **Confirmed successful forking**: The repository appeared under my account with all files and branches intact.

---

### 2. Cloning the Forked Repository
1. **Copied the repository URL**: From the "Code" dropdown, selected the SSH URL for the forked repository.
2. **Cloned it locally**: Opened my terminal and ran:
   ```bash
   git clone <repository-ssh-url>
   ```
3. **Navigated into the project directory**:
   ```bash
   cd <repository-name>
   ```

---

### 3. Setting Up the Environment
1. **Installed dependencies (if any)**: Followed the project-specific instructions (e.g., `npm install`, `pip install`).
2. **Opened the project in a code editor**: Used Visual Studio Code for easy editing and version control.

---

### 4. Making Changes
1. **Created a new branch**: Ensured isolation of my changes.
   ```bash
   git checkout -b <branch-name>
   ```
2. **Modified project files**: Updated content in a `README.md` and added a new feature in the code.
3. **Tracked changes**: Staged all updates using:
   ```bash
   git add .
   ```
4. **Committed changes**: Added a meaningful commit message:
   ```bash
   git commit -m "Updated README and added new feature"
   ```

---

### 5. Pushing Changes
1. **Pushed the branch to my fork**:
   ```bash
   git push -u origin <branch-name>
   ```
2. **Verified the updates on GitHub**: Confirmed the branch appeared in my forked repository.

---

### 6. Creating a Pull Request
1. **Navigated to my fork on GitHub**.
2. **Clicked "Compare & Pull Request"**: Selected the original repository as the base and my branch as the compare.
3. **Added PR details**: Documented the changes and provided context.
4. **Submitted the PR**: Awaited review and approval from the maintainers.

---

### 7. Keeping the Fork in Sync
1. **Added the original repository as upstream**:
   ```bash
   git remote add upstream <original-repo-ssh-url>
   ```
2. **Fetched updates**:
   ```bash
   git fetch upstream
   ```
3. **Merged updates into my fork**:
   ```bash
   git merge upstream/main
   ```

---

## Conclusion

This process allows effective collaboration and personal experimentation with open-source projects. The repository's history and contribution logs provide a detailed trace of changes for visibility and accountability. This workflow also ensures compatibility and ease of integration with the original repository.
