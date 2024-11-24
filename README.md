# Git Practice
Here’s a fun little exercise guide for Git beginners to practice the Git workflow. Each section includes steps as exercises with context to help learners understand the commands.

---

## **Git Beginner Practice Exercises**

### **1. Install Git**
Before you start, you need Git installed on your machine.

#### 📝 Exercise:
1. **Download Git**:
   - Visit [Git Downloads](https://git-scm.com/downloads) and download the version for your operating system.
2. **Install Git**:
   - Follow the installation steps for your OS.
3. **Verify Installation**:
   - Open your terminal and type:
     ```bash
     git --version
     ```
   - You should see the installed Git version.

---

### **2. Configure Your Git**
Learn how to personalize Git with your name and email.

#### 📝 Exercise:
```bash
git config user.name "Your Name"
git config user.email "your_email@example.com"
```
- What does this do? Sets your identity in the repository!

---

### **3. Clone and Explore a Repository**
Get hands-on with cloning a Git repository and exploring its contents.

#### 📝 Exercise:
```bash
git clone <repository_URL>
cd example-git-repo
ls
git status
```
- **Challenge**: What does `git status` tell you about your repo?

---

### **4. Add and Commit Files**
Understand the lifecycle of a file in Git.

#### 📝 Exercise:
1. Create a new file:
   ```bash
   touch about.html
   git status
   ```
2. Stage the file:
   ```bash
   git add about.html
   git status
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add an about file"
   git status
   ```

---

### **5. Edit and Commit Changes**
Learn to edit files and track changes in Git.

#### 📝 Exercise:
1. Add content to your file:
   ```bash
   echo "This is my about page" > about.html
   git status
   ```
2. Stage and commit the changes:
   ```bash
   git add about.html
   git commit -m "Update about page content"
   ```

---

### **6. Branching Basics**
Create, switch, and explore branches in your repository.

#### 📝 Exercise:
1. View and create branches:
   ```bash
   git branch
   git checkout -b add-about-page
   ```
2. Verify your branches:
   ```bash
   git branch
   git log --oneline
   ```

---

### **7. Merging Branches**
Practice merging changes from a branch into the main branch.

#### 📝 Exercise:
1. Switch to the main branch:
   ```bash
   git checkout master
   ```
2. Merge changes:
   ```bash
   git merge add-about-page
   git log --oneline
   ```

---

### **8. Staging and Amending**
Learn advanced commits by amending the last commit.

#### 📝 Exercise:
1. Stage a new file:
   ```bash
   touch products.html
   git add products.html
   ```
2. Amend your last commit:
   ```bash
   git commit --amend -m "Add products page"
   ```

---

### **9. Undoing Changes**
Master undoing accidental changes or commits.

#### 📝 Exercise:
1. "Accidentally" overwrite a file:
   ```bash
   echo "Oops content" > index.html
   git status
   ```
2. Restore the file:
   ```bash
   git restore -- index.html
   ```
3. Undo the last commit:
   ```bash
   git reset --soft HEAD~1
   ```

---

### **10. Stashing Work**
Learn to stash and restore changes.

#### 📝 Exercise:
1. Stash changes:
   ```bash
   git stash
   git status
   ```
2. Restore changes:
   ```bash
   git stash pop
   ```

---

### **11. Viewing Logs and Tags**
Explore Git logs and tag commits.

#### 📝 Exercise:
1. Add a tag to a commit:
   ```bash
   git tag 0.1.0
   git log --oneline
   ```
2. Add a new commit and check tags:
   ```bash
   touch new_file
   git add new_file
   git commit -m "Add new file"
   git log --oneline
   ```

---


With these interactive steps, you’ll master Git’s core functionality in no time! Practice often, and soon, Git will become second nature.
