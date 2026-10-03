Q1. What does --global mean, and what happens if you omit it?

The --global option applies the Git configuration to all repositories for the user. If --global is omitted, the configuration applies only to the current repository.

Q2. What appeared in ls -a but not ls, and what is inside it?

The .git directory appeared in ls -a because it is a hidden directory. It contains Git's repository information, including the history and configuration needed to manage the repository.

Q3. Roughly how many files/folders is Git offering to track? Is there anything you did not write?

Git was offering 4 files/folders to track: .DS_Store, .venv/, README.md, and week02/. The .DS_Store file and the files inside .venv/ were not written as part of my lab work.

Q4. Compare the status with Q3; what disappeared?

After adding the .gitignore file, .venv/ and .DS_Store disappeared from git status. Git is now ignoring these files and folders.

Q5. Should .gitignore itself be committed or ignored? Why?

The .gitignore file should be committed. It tells Git which files and folders should be ignored, so the repository needs to keep this file.

Q6. README moved between which two sections in git status? In the three-places model, what happened?

README.md moved from the "Untracked files" section to "Changes to be committed". In the three-places model, the file moved from the working directory to the staging area.

Q7. What did Git print after the commit; how many files changed?

Git printed the commit message "Lab work so far" and showed that 4 files changed with 81 insertions. The commit was created as the root commit.

Q8. What are the first seven characters of a commit called, and what are they for?

The first seven characters are a short form of the commit hash. They are used to identify a specific commit in the Git history.