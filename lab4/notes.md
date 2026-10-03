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

Q9. What are the four steps of the loop just repeated twice?

The four steps are edit the files, check the status, stage the changes, and commit the changes. We repeated this cycle to create separate Git commits for the lab work.

Q10. Why use the special name and place rather than notes.md?

README.md is special because GitHub displays it on the repository front page as an introduction to the project. It helps people understand what the repository contains.

Q11. What did gh auth login do so no password is needed on push?

The gh auth login command authenticates the GitHub CLI with my GitHub account. It allows Git to authenticate when pushing to GitHub without asking for my GitHub password.

Q12. What is on the front page of the GitHub repository, and why that file?

The front page shows the files and folders that were pushed to the repository. The README.md file is displayed as formatted text because GitHub uses it as the repository's main introduction.

Q13. Did the push change the local Git history?

No, pushing does not change the local Git history. It sends the existing local commits to the GitHub remote repository.

Q14. If the repository is private but TAs can read it, what is the difference between a private repo and no repo on GitHub?

A private repository is still hosted on GitHub, but only the owner and people who are given access can view it. With no repository on GitHub, the lab work is not available there for the TAs to access.