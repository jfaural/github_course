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

7. How to create and use a link between local and remote repository
   
   1. Create a link (bridge): `git remote add <name4link> <ssh key>`. The name for link is usually the same name as my repositories but ca be anything I like. It is just a name for the link that is being created.
   
   2. Send things from the local to your remote repository: `git push`

8. How to restore a local repository from the remote repository: `git clone <ssh key>`. You get the content, creates the local repository and creates the bridge between the local and the remore.

9. How to recover a deleted commit: `git reset` you can lose information, it is safer to use `git revert HEAD`, it reverts to the previous stage of the timeline. You can `git revert` the revert.

10. Helpful comment from Matilde

11. How to create a new branch `git branch <name>`

12. Save the same script with 5 different names, on the server, locally and in github and then never, ever find the 'good' version again. 

13. Dream of it forever, listfully staring at the one shitty version you seem to have saved everywhere
