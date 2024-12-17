# **Personal Finance Tracker - Team Guide**

### 🚀 **Branching Structure**

- **`main` branch**: Stable codebase. **No direct commits or merges** here.
- **`backend` branch**: For all backend development.
- **`frontend` branch**: For all frontend development.
- **Feature branches**:
  - Backend: `feature/<task-name>` (e.g., `feature/login-api`)
  - Frontend: `feature/<task-name>` (e.g., `feature/dashboard-ui`)

---

### 🛠️ **How to Work on the Project**

#### 1. **Always Pull Before Making Changes**

Before starting work:

```bash
git checkout <your-branch>
git pull origin <your-branch>
```

Example:

- For backend tasks: `git checkout backend && git pull origin backend`
- For frontend tasks: `git checkout frontend && git pull origin frontend`

---

#### 2. **Create a Feature Branch**

Work on a feature branch to keep your work isolated:

```bash
git checkout -b feature/<your-task-name>
```

Example:

```bash
git checkout -b feature/login-api
```

---

#### 3. **Commit and Push**

After completing your work:

```bash
git add .
git commit -m "Add <your feature/task>"
git push origin feature/<your-task-name>
```

---

#### 4. **Avoid Conflicts**

Before pushing, always pull the latest changes to avoid conflicts:

```bash
git pull origin <your-branch>
```

If conflicts occur:

- **Abort Changes**: Use `git merge --abort` if you made a mistake.
- **Resolve Manually**: Compare changes, fix conflicts, and ensure everyone’s code is intact.

**Do not overwrite other team members' work!**

---

#### 5. **No Direct Merge to `main`**

- Backend team works on the **`backend`** branch.
- Frontend team works on the **`frontend`** branch.
- **Never merge your branches into `main`**.

**Final merging** will be done **at the end of the project** during submission.

---

### ✅ **Summary Workflow**

1. Pull the latest code from your branch (`backend` or `frontend`).
2. Create a feature branch: `feature/<your-task-name>`.
3. Work on your task, commit, and push.
4. Pull changes before pushing to avoid conflicts.
5. Resolve conflicts carefully without overwriting others' work.

---

### 🚨 **Important Reminders**

- Always communicate with your team.
- Use **clear commit messages** to describe your changes.
- Keep backend and frontend work **separate**.
