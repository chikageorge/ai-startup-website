# PART 2: Simulating Tom and Jerry's Work

This guide will walk you through the basics of using GitHub, including navigating a project directory, creating branches, making changes, and collaborating with others. We'll simulate workflows for two contributors, Tom and Jerry.

---

## Navigating the Project Directory and Checking Branches

### Steps:
1. **Navigate to the project directory** you just cloned using the command:
   ```bash
   cd ai-startup-web
   ```

2. **Check the current branch in the repository** using:
   ```bash
   git branch
   ```

   This will display all the branches in the repository.

3. **Create a new branch called `update-navigation`:**
   ```bash
   git checkout -b update-navigation
   ```

4. **Verify the new branch** by running `git branch` again. You should see the newly created branch listed.

![Git branching](images/git-Navigating.PNG)

---

## Making Changes and Staging Them

### Steps:
1. Open the `index.html` file in your code editor. Since this file already exists in the main branch, it will also exist in the new branch you created.

2. Add the following content to the `index.html` file:
   ```html
   This is Tom adding Navigation to the AI-website
   ```
   ![Git Status](images/new-branch-index.PNG)

3. **Check the status of your changes** using:
   ```bash
   git status
   ```

   This will show that the changes have not been staged yet.

4. **Stage the changes** using:
   ```bash
   git add .
   ```

5. **Confirm the staged changes** by running `git status` again. The changes should now be staged and ready to commit.

![Git Status](images/staging-status.PNG)

---

## Committing and Pushing Changes

### Steps:
1. **Commit the changes** with a meaningful message:
   ```bash
   git commit -m "update navigation bar"
   ```
   ![Git Status](images/Branch-commit.PNG)

2. **Push the branch to GitHub** using:
   ```bash
   git push origin update-navigation
   ```
   ![Git Status](images/Branch-push.PNG)

---

## Simulating Jerry's Contribution

### Steps:
1. **Switch back to the main branch**:
   ```bash
   git checkout main
   ```

2. **Create a new branch for Jerry called `add-contact-info`:**
   ```bash
   git checkout -b add-contact-info
   ```

3. Make the necessary changes to the project (e.g., adding contact information to `index.html`).

4. **Stage, commit, and push Jerry's changes:**
   ```bash
   git add .
   git commit -m "add contact information"
   git push origin add-contact-info
   ```
   ![Git Status](images/git-status-Screenshot%202025-03-16%20171638.png)

---
## Part 3: Merging Changes

### Steps:
1. **Switch to Update-navigation branch**:
   ![Git Status](images/change-branch1.png)

2. **Create New Pull Request**
   ![Git Status](images/create-pull-request.png)

   ![Git Status](images/comment-to-pull-request3.png)

---
## Updating Jerry's Branch with latest changes

### Steps:
1. **Switch to Jerry's Branch**:
   ```bash
   git checkout add-contact-info
   ```
    ![Git Status](images/check-out-add-contact.png)
2. **Pull the changes from the main branch**
    ```bash
   git pull origin main
   ```
<<<<<<< HEAD
   ![Git Status](images/pull-request-to-update-add-contact.png)
=======
    ![Git Status](images/pull-request-to-update-add-contact.png)
>>>>>>> ca6336a22ce5e12898a554b449978eea660a644d
---
## Finalizing Jerry's Contribution

### Steps:
1. **Push the updated version to giihub**:
   ```bash
   git push origin add-contact-info
   ```
---
