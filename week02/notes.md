1.⁠ ⁠What did pwd print?
Ans.bojjaprasanth@BOJJAs-MacBook-Air ~ % pwd
/Users/bojjaprasanth

2.⁠ ⁠What did ls -a show that plain ls did not?
Ans. ls -a showed hidden files like . and .. that normal ls didn't show.

3.⁠Pick one line from ls -l. What do you think the first column means?
Line selected: -rw-r--r--@   1 bojjaprasanth  staff     33 Jul  4 18:20 1st CODE
shows the file permissions, meaning the owner, group, and others can read and execute this file, but no one can write to it.

4.⁠ ⁠Why does that work from where you are standing? Which kind of path is coding-cafe/week02? Absolute or Relative?
Ans. It works because we are already inside the coding-cafe folder, so we can directly use coding-cafe/week02 without giving the full path. It is a relative path because it starts from the current folder, not from the root directory.

5.  mv did two different jobs above. What were they?
Ans. The mv command performed these two distinct jobs in your terminal:
Moving a file: In the first instance (mv README-backup.md week01/), it relocated the file from your current folder into the week01 folder.
Renaming a file: In the second instance (mv README-backup.md old-readme.md), it changed the name of the file without changing its location.

6.⁠ ⁠How many folders are on your PATH? (They are separated by :)
Ans. There are 15 folders in my path there are,
    /Users/bojjaprasanth/Library/Application Support/Code/User/globalStorage/github.copilot-chat/debugCommand:/Users/bojjaprasanth/Library/Application Support/Code/User/globalStorage/github.copilot-chat/copilotCli:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/pkg/env/global/bin:/opt/homebrew/bin:/Users/bojjaprasanth/Library/Application Support/Code/User/globalStorage/github.copilot-chat/debugCommand:/Users/bojjaprasanth/Library/Application Support/Code/User/globalStorage/github.copilot-chat/copilotCli

7.⁠ ⁠Write down exactly where your python3 lives. You will need this again in a minute.
bojjaprasanth@BOJJAs-MacBook-Air week01 % which python3
/usr/bin/python3

8.⁠ ⁠Compare your answer to 7 with the person next to you. Are they the same? If not, why might that be?
Ans. Yes it would be same, If that is different the other person may have downloaded the python by using the different package manager or environmnt which places Python in a different path. 

9.⁠ ⁠What exactly did the shell say? Explain the error in your own words, using the word PATH.
bojjaprasanth@BOJJAs-MacBook-Air week01 % pyton3
zsh: command not found: pyton3
This should show that the shell had searched for the pyton 3 but couldn't find it listed in my PATH variable. Instead it gave me a suggestion that it might be python3.

10. Why .venv did not appear with plain ls Why not? (Refer back to section 1.)
Ans. `.venv` is a hidden directory because its name starts with a period (`.`). Plain `ls` ignores hidden files and directories unless you use the `-a` flag (`ls -a`).

11. What changed about your prompt?
Ans. The prompt now has `(.venv)` prepended at the very beginning, indicating that the virtual environment is currently active.

12. Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell you about what activate actually did to your PATH?
Ans. /home/bojjaprasanth/coding-cafe/.venv/bin/python3
No, it is not the same path. Question 7 pointed to `/usr/bin/python3`, but now it points to `/home/bojjaprasanth/coding-cafe/.venv/bin/python3`. This tells me that `activate` prepended the `.venv/bin` directory to the very front of my `PATH` variable, forcing the shell to find and use the virtual environment's Python before the global system Python.

13. What is in the second list that was not in the first?
Ans. The second list contains requests and its dependencies (certifi, charset-normalizer, idna, and urllib3) which were installed after running `pip install requests`.

14. Where does python3 point now?
Ans. /usr/bin/python3

15.  Find what ls -h does. Write it in your own words
Ans.  -h, --human-readable
              Print human readable file sizes (e.g. 1K 234M 56G).
The `ls -h` flag prints file sizes in human-readable units (such as 1K, 234M, or 2G) instead of listing them in raw bytes, making the output much easier to understand when viewing file listings like `ls -l`.

16. What is the difference between what Ctrl + C and Ctrl + D did?
Ans. Ctrl+C sends an interrupt signal (SIGINT) to cancel or forcefully terminate a running command immediately, whereas Ctrl+D sends an End-Of-File (EOF) marker to indicate that input has ended, allowing Python or the shell to exit cleanly.


