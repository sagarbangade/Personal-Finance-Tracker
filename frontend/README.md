# Frontend Team Guidelines

Welcome to the frontend folder! This file contains guidelines for working on the **frontend** codebase.

---

## **Branch Workflow**

1. **Base Branch**:

   - The `frontend` branch is the base branch for all frontend work.
   - Always pull the latest changes from the `frontend` branch before starting new work.

2. **Creating a Feature Branch**:

   - For each new feature, create a **feature branch** from the `frontend` branch:
     ```bash
     git checkout frontend
     git pull origin frontend  # Ensure you have the latest changes
     git checkout -b feature/<feature-name>
     ```
   - Use meaningful names for feature branches, e.g.:
     - `feature/login-page`
     - `feature/dashboard-ui`

3. **Working on Your Feature**:

   - Commit your changes regularly with clear messages:
     ```bash
     git add .
     git commit -m "Add login form UI"
     ```

4. **Pushing Your Feature Branch**:

   - Push your feature branch to the remote repository:
     ```bash
     git push origin feature/<feature-name>
     ```

5. **Merging Back to `frontend`**:

   - When your feature is complete, create a **pull request** (PR) to merge your feature branch into the `frontend` branch.
   - **Do NOT merge your branch directly**. Wait for code review approval.

6. **Pull Latest Before New Work**:
   - Always pull the latest changes in the `frontend` branch before starting new work:
     ```bash
     git checkout frontend
     git pull origin frontend
     ```

---

## **Folder Structure**

```plaintext
frontend/
│
├── public/          # Static assets
├── src/             # React or frontend source code
│   ├── components/  # Reusable UI components
│   ├── pages/       # Page-specific components
│   ├── utils/       # Utility functions
│   └── App.js
│
└── package.json     # Node.js dependencies
```

---

## **Example Workflow**

1. Pull the latest changes from `frontend`:

   ```bash
   git checkout frontend
   git pull origin frontend
   ```

2. Create a new feature branch:

   ```bash
   git checkout -b feature/navbar-component
   ```

3. Work on your feature and commit changes:

   ```bash
   git add .
   git commit -m "Add responsive navbar component"
   ```

4. Push your branch and create a PR:
   ```bash
   git push origin feature/navbar-component
   ```

---

**Remember**: Do not merge directly into `frontend`. Always use a pull request to maintain clean and reviewed code. 🚀
