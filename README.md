## GitHub Workflow Guide for Beginners

### 1. Fork a Repository
- Visit the GitHub page of the public repository you want to fork.
- Click the "Fork" button in the top-right corner of the page.

### 2. Clone the Repository Locally
- Open your terminal or command prompt.
- Clone your forked repository:
  ```bash
  git clone https://github.com/your-username/repository-name.git
- Navigate into the cloned directory:
```bash
cd repository-name
```

### 3. Write Code
Make changes to the code using your text editor or IDE.

### 4. Commit Changes
```bash
git add .
git commit -am "Your commit message"
```

### 5. Push Changes to Your Fork
```bash
git push origin master
```
Set the upstream branch for future pushes (only needed once):
```bash
git push -u origin master
```

### 6. Setting Up GitHub Authentication
- Go to Settings -> Developer Settings -> Personal Access Tokens
- Generate Classic Personal Access Token
- Save on your computer
- When you push to GitHub from the terminal, copy and paste your PAT as your password
