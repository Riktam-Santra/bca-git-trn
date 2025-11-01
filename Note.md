# 🪴 Creating a New Branch in Git

## 🔹 What is a Branch?
A branch in Git is like a separate workspace where you can develop new features, fix bugs, or experiment — without affecting the main code (usually `main` or `master` branch).

---

## ⚙️ Steps to Create and Use a New Branch

### 🧩 1. Check current branch
```bash
git branch
```
Lists all branches and shows which one you’re currently on (with a `*` mark).

---

### 🌱 2. Create a new branch
```bash
git branch feature-branch
```
Creates a branch named `feature-branch`.


---

### 🔄 3. Switch to that branch
```bash
git checkout feature-branch
```
Or, in newer Git versions (recommended):
```bash
git switch feature-branch
```
Now, you’re working *inside* the new branch.

---

### 🛠️ 4. Make changes and commit
```bash
git add .
git commit -m "Added new feature"
```

---

### ⬆️ 5. Push your new branch to remote (like GitHub)
```bash
git push origin feature-branch
```
Uploads your new branch to the remote repository.

---

### 📂 6. Switch back to main branch
```bash
git switch main
```
(or `git checkout main`)

---

### 🧹 7. (Optional) Delete branch after merging
Once your changes are merged:
```bash
git branch -d feature-branch
```
To delete it from remote too:
```bash
git push origin --delete feature-branch
```

---

## ✅ Summary

| Command | Description |
|----------|--------------|
| `git branch <name>` | Create a branch |
| `git switch <name>` | Move to that branch |
| `git push origin <name>` | Upload branch to GitHub |
| `git branch -d <name>` | Delete local branch |
| `git push origin --delete <name>` | Delete remote branch |
