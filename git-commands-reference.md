
# Git Commands Quick Reference

## Initializing and Configuring a Repository

### Initialize a Git repository
```bash
git init
```

### Clone a repository
```bash
git clone <repository-url>
```

### Set user name and email
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

## Staging and Committing Changes

### Add a file to the staging area
```bash
git add <file>
```

### Add all files to the staging area
```bash
git add .
```

### Commit changes
```bash
git commit -m "Commit message"
```

### Add and commit in one step
```bash
git commit -am "Commit message"
```

---

## Branching and Merging

### Create a new branch
```bash
git branch <branch-name>
```

### Switch to another branch
```bash
git checkout <branch-name>
```

### Create and switch to a new branch
```bash
git checkout -b <branch-name>
```

### Merge a branch into the current branch
```bash
git merge <branch-name>
```

---

## Working with Remotes

### Add a remote repository
```bash
git remote add origin <repository-url>
```

### List remote repositories
```bash
git remote -v
```

### Remove a remote repository
```bash
git remote remove <remote-name>
```

---

## Pulling and Pushing Changes

### Push changes to a remote repository
```bash
git push origin <branch-name>
```

### Pull changes from a remote repository
```bash
git pull origin <branch-name>
```

---

## Viewing History and Status

### View commit history
```bash
git log
```

### View the status of your working directory
```bash
git status
```

### Show differences between working directory and staging area
```bash
git diff
```

---

## Undoing Changes

### Unstage a file
```bash
git reset <file>
```

### Revert changes in the working directory
```bash
git checkout -- <file>
```

### Amend the last commit
```bash
git commit --amend
```

---

## Deleting Branches

### Delete a local branch
```bash
git branch -d <branch-name>
```

### Delete a remote branch
```bash
git push origin --delete <branch-name>
```

---

## Tagging

### Create a tag
```bash
git tag <tag-name>
```

### Push a tag to the remote repository
```bash
git push origin <tag-name>
```

### List all tags
```bash
git tag
```

---

## Help

### Display help for a specific command
```bash
git <command> --help
```

