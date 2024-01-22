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
git commit -m "Your commit message"
```

### 5. Push Changes to Your Fork
```bash
git push origin main
```
Set the upstream branch for future pushes (only needed once):
```bash
git push -u origin main
```

### 6. Setting Up GitHub Authentication
Generate a new SSH key (or use an existing one):
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
Add your SSH key to the ssh-agent:
```
```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```
Copy the SSH key to your clipboard:

For Windows:
```bash
clip < ~/.ssh/id_ed25519.pub
```
For Mac:
```bash
pbcopy < ~/.ssh/id_ed25519.pub
```
Add the SSH key to your GitHub account:

Go to GitHub and navigate to your account settings.
Click on "SSH and GPG keys" and then "New SSH key".
Paste your key and save it.

Test your SSH connection:
```bash
ssh -T git@github.com
```
