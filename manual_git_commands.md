# Manual of git commands

1. How to initialize git
   
   `git init`

2. How to send to the staging area
   
   `git add <file_name>`
   
   How to use it cleaverly: use `git status` to check before you commit, `git add <file_1> <file_2>`

3. how to commit a change to create my 1st snapshot
   
   `git commit -m "MEANINGFUL MESSAGE"`
   
   Meaningful means: why, how, limitations and effects.
   
   4. How to check in what conceptual areas my files are:
   
   `git status`

               It will tell me uncommited, unstaged and untracked files.

Testing what happens if I don't use -m to commit

5. How to see the history of my timeline:
   
   `git log`
   
   With no arguments, `git log` lists the commits made in that repository in reverse chronological order. If you use `-p` or `--patch`, it will show the difference (the *patch* output) introduced in each commit. You can also limit the number of log entries displayed, such as using `-2` to show only the last two entries. You can also change the format with `--pretty` (example `--pretty=oneline`). `--abbrev-commit` to have a shorter verion of the commit id.

6. How can I travel within the timeline to check for differences in my versions? It is important which one you put first, because it is going to be one minus the other. You can see the commit id with `git log`. Or with `git show -2` you can see the last 2 versions.

        `git diff <commit_id1> <commit_id2>`
