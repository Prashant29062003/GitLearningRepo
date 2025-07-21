# Git Cheat Sheet


---

The Git Cheat Sheet is a concise, categorized guide for developers and DevOps engineers, covering Git basics to advanced topics. It includes installation, configuration, commands, branching, merging, and more.

---

## 🔧 Git Installation Commands

| Command                               | Description                          |
| ------------------------------------- | ------------------------------------ |
| Git for Windows stand-alone installer | Download and install Git for Windows |
| `brew install git`                    | Install Git with Homebrew on Mac OS  |
| `sudo port selfupdate`                | Install Git with MacPorts on Mac OS  |
| `sudo apt-get install git`            | Install Git on Linux                 |
| `git --version`                       | Check installed Git version          |

---

## 📅 Git Configuration & Setup

| Command                                                  | Description                      |
| -------------------------------------------------------- | -------------------------------- |
| `git config --global user.name "Your Name"`              | Set global Git username          |
| `git config --global user.email "youremail@example.com"` | Set global Git email address     |
| `git config --global color.ui auto`                      | Enable colored terminal output   |
| `git config --global alias.<alias> <git-command>`        | Create Git command alias         |
| `git config --list`                                      | List Git configuration settings  |
| `git config --get <key>`                                 | Get specific configuration value |
| `git help`                                               | Show help documentation          |

---

## 🔄 Initializing a Repository

| Command                             | Description                          |
| ----------------------------------- | ------------------------------------ |
| `git init`                          | Initialize a new Git repository      |
| `git init <directory>`              | Create a repo in specified directory |
| `git clone <repository_url>`        | Clone a repo from remote             |
| `git clone --branch <branch> <url>` | Clone a specific branch              |

---

## ⚖️ Basic Git Commands

| Command                           | Description                              |
| --------------------------------- | ---------------------------------------- |
| `git add <file>`                  | Stage a file                             |
| `git add .` or `git add --all`    | Stage all modified/new files             |
| `git status`                      | Show repo status                         |
| `git status --ignored`            | Include ignored files in status          |
| `git diff`                        | Show unstaged changes                    |
| `git diff <commit1> <commit2>`    | Compare two commits                      |
| `git diff --staged` or `--cached` | Compare staged with last commit          |
| `git diff HEAD`                   | Show changes since last commit           |
| `git commit`                      | Commit staged changes                    |
| `git commit -m "msg"`             | Commit with inline message               |
| `git commit -a`                   | Commit all modified/deleted files        |
| `git notes add`                   | Add note to object                       |
| `git restore <file>`              | Restore file from last commit            |
| `git reset <commit>`              | Reset to a commit                        |
| `git reset --soft <commit>`       | Reset but keep changes staged            |
| `git reset --hard <commit>`       | Reset and discard changes                |
| `git rm <file>`                   | Remove file from repo and stage deletion |
| `git mv <old> <new>`              | Rename or move file                      |

---

## 📃 Git Commit Types

| Command                             | Description             |
| ----------------------------------- | ----------------------- |
| `git commit -m "feat: message"`     | New feature             |
| `git commit -m "fix: message"`      | Bug fix                 |
| `git commit -m "chore: message"`    | Maintenance             |
| `git commit -m "refactor: message"` | Code refactoring        |
| `git commit -m "docs: message"`     | Documentation change    |
| `git commit -m "style: message"`    | Code formatting/styling |
| `git commit -m "test: message"`     | Test changes            |
| `git commit -m "perf: message"`     | Performance improvement |
| `git commit -m "ci: message"`       | CI-related change       |
| `git commit -m "build: message"`    | Build process update    |
| `git commit -m "revert: message"`   | Revert previous commit  |

---

## 📖 Branching & Merging

| Command                     | Description                     |
| --------------------------- | ------------------------------- |
| `git branch`                | List local branches             |
| `git branch <name>`         | Create new branch               |
| `git branch -d <name>`      | Delete a branch                 |
| `git branch -a`             | List local and remote branches  |
| `git branch -r`             | List remote branches            |
| `git checkout <name>`       | Switch to branch                |
| `git checkout -b <name>`    | Create and switch to branch     |
| `git checkout -- <file>`    | Discard changes in file         |
| `git merge <branch>`        | Merge a branch into current     |
| `git log`                   | Show commit history             |
| `git log --follow <file>`   | Show file history incl. renames |
| `git stash`                 | Temporarily save changes        |
| `git stash list`            | Show saved stashes              |
| `git stash pop`             | Apply & remove last stash       |
| `git stash drop`            | Remove last stash               |
| `git tag`                   | List all tags                   |
| `git tag <tag>`             | Create tag at current commit    |
| `git tag -a <tag> -m "msg"` | Create annotated tag            |

---

## 💾 Remote Repositories

| Command                         | Description                  |
| ------------------------------- | ---------------------------- |
| `git fetch`                     | Retrieve changes from remote |
| `git pull`                      | Fetch and merge from remote  |
| `git pull --rebase`             | Rebase instead of merge      |
| `git push`                      | Push to remote               |
| `git push --all`                | Push all branches            |
| `git remote`                    | List remotes                 |
| `git remote add <name> <url>`   | Add remote                   |
| `git remote rm <name>`          | Remove remote                |
| `git remote rename <old> <new>` | Rename remote                |

---

## 🔄 Git Comparison

| Command             | Description               |
| ------------------- | ------------------------- |
| `git show`          | Show commit changes       |
| `git show <commit>` | Show specific commit info |

---

## 🔎 Logging & Reviewing

| Command                         | Description             |
| ------------------------------- | ----------------------- |
| `git log`                       | View commit history     |
| `git log --oneline`             | Compact history         |
| `git log --graph`               | ASCII graph view        |
| `git log --author="Name"`       | Filter by author        |
| `git log --since="2 weeks ago"` | Recent commits          |
| `git log --until="date"`        | Older commits           |
| `git log <file>`                | File commit history     |
| `git blame <file>`              | Line-by-line authorship |
| `git diff`                      | Show unstaged changes   |
| `git diff --staged`             | Show staged changes     |
| `git diff <c1> <c2>`            | Compare commits         |

---

## ⏲️ Managing Git History

| Command                           | Description                              |
| --------------------------------- | ---------------------------------------- |
| `git revert <commit>`             | Undo changes via new commit              |
| `git revert --no-commit <commit>` | Undo without committing                  |
| `git rebase <branch>`             | Reapply commits on top of another branch |

---

## 🧐 Git Reflog

| Command                     | Description                 |
| --------------------------- | --------------------------- |
| `git reflog`                | Show HEAD changes history   |
| `git checkout HEAD@{n}`     | Restore previous HEAD state |
| `git reset --hard HEAD@{n}` | Hard reset to past state    |

---
