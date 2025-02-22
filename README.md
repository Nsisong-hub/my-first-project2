# command-line-basics
## Introduction
This assignment demonstrates the fundamental operations of Git and command-line interactions, including repository initialization, file creation, tracking changes, and pushing to GitHub
## Prerequisites
* Installed Git
* GitHub account
* Basic knowledge of Git commands
* A terminal (Git Bash for Windows, Linux terminal, or macOS Terminal)
## Steps Performed and Commands Used
**1. Setting Up the Project Directory**
* A new directory Assignment2 is created inside the projects folder
```bash
cd projects/
mkdir Assignment2
cd Assignment2
```
<img width="1106" alt="image" src="https://github.com/user-attachments/assets/29ede0eb-66dc-4385-9257-0e03a3b8ca1c" />

**2. Initialize Git repository: \`git init\`**
* This initializes an empty Git repository in Assignment2

```bash
git init
```
<img width="1106" alt="image" src="https://github.com/user-attachments/assets/4f0800b6-940d-4deb-ad6e-1d2b5cca8da7" />

**3. Creating Files**
* I created Two files (file1 and file2) and verified using the ls command
```bash
touch file1 file2
ls
```
<img width="1106" alt="image" src="https://github.com/user-attachments/assets/b9b5088a-0a25-403b-9f0b-b657fcd767ce" />

**4. Checking Git Status**
* This command checks the status of the working directory and lists untracked files
```bash
git status
```
<img width="1117" alt="image" src="https://github.com/user-attachments/assets/4a56adc7-ffed-409a-83af-ba5248a6ee80" />

**5. Staging Files**

* This stages all untracked files for the next commit
  
```bash
git add .
```
<img width="1104" alt="image" src="https://github.com/user-attachments/assets/3dfc9f7c-3853-4825-9300-07f88a004012" />

**6. Committing Changes**
* This commits the staged files with a message "Initial commit"
```bash
git commit -m "Initial commit"
```
<img width="1103" alt="image" src="https://github.com/user-attachments/assets/47e0bc8c-e2a6-446a-a85c-540c33a272b8" />

**7. Adding a Remote Repository**
* This links the local repository to a remote GitHub repository
  
```bash
git remote add origin https://github.com/Nsisong-hub/my-first-project2.git
```
<img width="1106" alt="image" src="https://github.com/user-attachments/assets/9e1417c1-5ae9-4c4a-b84a-1d3e5d72fd70" />

**8. Pushing to GitHub**
* The initial push was rejected due to remote changes, leading to a rebase
```bash
git push -u origin master
```
**9. Resolving Push Issues with Rebase**
* I performed a rebase to integrate remote changes before pushing successfully
```bash
git pull --rebase origin master
git push -u origin master
```
<img width="1116" alt="image" src="https://github.com/user-attachments/assets/23bd4226-94cb-40b4-a524-63efcb4ab8fa" />

**10. Cloning the Repository to a New Folder**
* Created a new folder and cd into it
* Then cloned a fresh copy of the repository into the Newfolder
```bash
mkdir Newfolder
cd Newfolder
git clone https://github.com/Nsisong-hub/my-first-project2.git
```
<img width="1106" alt="image" src="https://github.com/user-attachments/assets/fb644617-e5e0-42ac-aa56-6561c687f1ff" />

**11. Adding a New File**
* I Created a new file goals.txt with programming goals
```bash
echo "My programming goals:
- Learn Git and GitHub
- Master Python
- Build cloud-based applications
" > goals.txt
ls
```
<img width="1104" alt="image" src="https://github.com/user-attachments/assets/750e77cb-5d64-49c6-ac5f-b359ad4e804b" />

**12. Tracking and Committing goals.txt**

* The new file was added, committed, and pushed to the remote repository
  
```bash
git add goals.txt
git commit -m "Added goals.txt"
git push origin master
```

<img width="1105" alt="image" src="https://github.com/user-attachments/assets/bc5656a8-08a1-4bcc-81f8-868ff867c4a7" />

<img width="1106" alt="image" src="https://github.com/user-attachments/assets/2f90309b-eff2-4b9d-af15-d973e04c1b8a" />



## Conclusion

This assignment covers key Git operations such as:

* Repository initialization

* File creation and tracking

* Handling remote repositories

* Resolving push conflicts with rebase

* Cloning repositories

This provides a strong foundation for version control using Git and GitHub.





