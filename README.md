# PLPBasicGitAssignment
Certainly! Here are the detailed steps for completing the tasks, followed by a summary of the issues/errors encountered and how they were resolved.

### Task 2: Local Setup

#### Step 2.1: Create a New Folder
1. Open a terminal.
2. Create a new folder and navigate into it:
    ```bash
    mkdir PLPBasicGitAssignment
    cd PLPBasicGitAssignment
    ```

#### Step 2.2: Git Initialization
1. Initialize a new Git repository in the local folder:
    ```bash
    git init
    ```

#### Step 2.3: Connecting to GitHub
1. Link your local repository to the GitHub repository:
    ```bash
    git remote add origin https://github.com/dantekadagi3/PLPBasicGitAssignment.git
    ```

### Task 3: Making Changes

#### Step 3.1: Create a File
1. Create a new text file and add a simple text message:
    ```bash
    echo "Hello, Git!" > hello.txt
    ```

#### Step 3.2: Committing Changes
1. Stage the changes:
    ```bash
    git add hello.txt
    ```
2. Commit the changes:
    ```bash
    git commit -m "Add hello.txt with a greeting"
    ```

### Task 4: Pushing to GitHub

#### Step 4.1: Pushing to GitHub
1. Push the committed changes to your GitHub repository:
    ```bash
    git push -u origin main
    ```

### Task 5: Verification

#### Step 5.1: Verify on GitHub
1. Visit your GitHub repository in a web browser and confirm that the `hello.txt` file and commit message are visible.

### Issues/Errors and Resolutions

#### Issue 1: No such file or directory
- **Error Message**: `bash: cd: PLPBasicGitAssignment: No such file or directory`
- **Resolution**: Ensure you are in the correct directory. If you get this error after trying to navigate into the directory, make sure the directory name is correct and exists.

#### Issue 2: Pathspec 'hello.txt' did not match any files
- **Error Message**: `fatal: pathspec 'hello.txt' did not match any files`
- **Resolution**: Ensure the file `hello.txt` exists in the current directory and is spelled correctly.

#### Issue 3: Commit message syntax error
- **Error Message**: `error: unknown switch 'A'`
- **Resolution**: Use the correct syntax for the commit message:
    ```bash
    git commit -m "Add hello.txt with a greeting"
    ```

#### Issue 4: Author identity unknown
- **Error Message**: `fatal: unable to auto-detect email address`
- **Resolution**: Configure your Git user details:
    ```bash
    git config --global user.email "dantekadagi3@gmail.com"
    git config --global user.name "dantekadagi3"
    ```

#### Issue 5: Branch name mismatch
- **Error Message**: `error: src refspec main does not match any`
- **Resolution**: Ensure your local branch is named correctly and exists. Rename `master` to `main` if necessary:
    ```bash
    git branch -m master main
    ```

#### Issue 6: Authentication failure
- **Error Message**: `remote: Support for password authentication was removed on August 13, 2021.`
- **Resolution**: Use a Personal Access Token (PAT) for authentication instead of a password.

#### Issue 7: Remote contains work you do not have locally
- **Error Message**: `error: failed to push some refs to 'https://github.com/dantekadagi3/PLPBasicGitAssignment.git'`
- **Resolution**: Pull the changes from the remote repository and rebase:
    ```bash
    git pull origin main --rebase
    ```

### Summary of All Steps:

1. Create a new folder:
    ```bash
    mkdir PLPBasicGitAssignment
    cd PLPBasicGitAssignment
    ```
2. Initialize a Git repository:
    ```bash
    git init
    ```
3. Link to the remote repository:
    ```bash
    git remote add origin https://github.com/dantekadagi3/PLPBasicGitAssignment.git
    ```
4. Create and add a text file:
    ```bash
    echo "Hello, Git!" > hello.txt
    git add hello.txt
    ```
5. Commit the changes:
    ```bash
    git commit -m "Add hello.txt with a greeting"
    ```
6. Configure Git user details:
    ```bash
    git config --global user.email "dantekadagi3@gmail.com"
    git config --global user.name "dantekadagi3"
    ```
7. Rename the branch if necessary:
    ```bash
    git branch -m master main
    ```
8. Pull changes and rebase:
    ```bash
    git pull origin main --rebase
    ```
9. Push the changes:
    ```bash
    git push -u origin main
    ```

Note:I had already created a github repository hence the steps for that are not included here
