# Backend Team Guidelines

Welcome to the backend folder! This file contains guidelines for working on the **backend** codebase.

---

## **Branch Workflow**

1. **Base Branch**:

   - The `backend` branch is the base branch for all backend work.
   - Always pull the latest changes from the `backend` branch before starting new work.

2. **Creating a Feature Branch**:

   - For each new feature, create a **feature branch** from the `backend` branch:
     ```bash
     git checkout backend
     git pull origin backend  # Ensure you have the latest changes
     git checkout -b feature/<feature-name>
     ```
   - Use meaningful names for feature branches, e.g.:
     - `feature/user-authentication`
     - `feature/expense-api`

3. **Working on Your Feature**:

   - Commit your changes regularly with clear messages:
     ```bash
     git add .
     git commit -m "Implement user login API"
     ```

4. **Pushing Your Feature Branch**:

   - Push your feature branch to the remote repository:
     ```bash
     git push origin feature/<feature-name>
     ```

5. **Merging Back to `backend`**:

   - When your feature is complete, create a **pull request** (PR) to merge your feature branch into the `backend` branch.
   - **Do NOT merge your branch directly**. Wait for code review approval.

6. **Pull Latest Before New Work**:
   - Always pull the latest changes in the `backend` branch before starting new work:
     ```bash
     git checkout backend
     git pull origin backend
     ```

---

## **Folder Structure**

```plaintext
backend/
│
├── controllers/     # Route controllers (business logic)
├── models/          # Database models
├── routes/          # API routes
├── middleware/      # Middleware (e.g., auth, error handling)
├── config/          # Configurations (e.g., DB connection)
├── utils/           # Utility functions
├── server.js        # Entry point for the backend
│
└── package.json     # Node.js dependencies
```

---

## **Example Workflow**

1. Pull the latest changes from `backend`:

   ```bash
   git checkout backend
   git pull origin backend
   ```

2. Create a new feature branch:

   ```bash
   git checkout -b feature/user-authentication
   ```

3. Work on your feature and commit changes:

   ```bash
   git add .
   git commit -m "Add JWT-based user authentication"
   ```

4. Push your branch and create a PR:
   ```bash
   git push origin feature/user-authentication
   ```

---

**Remember**: Do not merge directly into `backend`. Always use a pull request to maintain clean and reviewed code. 🚀

```

---

### Key Notes for Both Teams
- **Avoid Conflicts**: Always pull the latest changes from your base branch before starting or pushing work.
- **Feature Branches**: Use the naming convention `feature/<feature-name>`.
- **No Direct Merges**: Do not merge directly into `frontend` or `backend`. Use Pull Requests.
- **Code Reviews**: Wait for at least one team member to review and approve your PR before merging.

```
