# 🧪 Git Commands

### ➕ `git add`

Adds files to staging area

```bash
git add file.txt
git add .
git add --all
git add *.txt
git add docs/
```

---

### ✅ `git commit`

Commits staged files with a message

```bash
git commit -m "Your message"
```

---

### 📤 `git push`

Sends local commits to remote repo

```bash
git push -u origin master
```

---

### 📥 `git pull`

Fetches & merges changes from remote

```bash
git pull
```

---

## 🛠 Additional Git Commands:

| Command        | Use                                             |
| -------------- | ----------------------------------------------- |
| `git status`   | Shows current status (tracked, untracked, etc.) |
| `git log`      | Shows commit history                            |
| `.gitignore`   | Hides files from Git                            |
| `git merge`    | Merges branches/repos                           |
| `git checkout` | Switches versions or branches                   |

---

## 📌 Example Git Flow

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin <repo-url>
git push -u origin master
```

---
