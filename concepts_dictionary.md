# My 1st Github project

What is a Git repository? It is where you can store your project and make modifications, all the versions will be stored there. Also, single collection of documents where you want to track modifications. It can be online or offline. 

What is Github? It is a collection of all your Git repositories. It is online.

### Conceptual areas

1. Developing area: the folder where you initialized git and where the project is developed. It is in your computer locally.

2. Staging area: where you are going to get what you want to make a snapshot of. While it is in this area, you can still make changes, it is an intermediate area. Location to prepare new snapshots to the timeline. To get there, git add goes from the developing area to the staging area. From the developing area to the local repository, this also happens locally. `git add` to send things to the staging area.
   
   OBS: Why to use the staging area? The staging area is important because you can commit files together. You can track parallel changes together.

3. Local repository: where you save your snapshots. The `.git` is your local repository, it is a hidden folder. If you delete the file, you delete your local repository. You can use `ls -la` to visualize your `.git` folder. It is also in my computer - locally. P.s: you can do `git status `to check the location of the files.

4. Remote repository: github. We have to create a link between the git repository and github. This most likely a clour-like kind of repository. In this case it is represented by GitHub. 

`README.txt`: detailed description of your project and tool usage (if it is the case)

`.gitignore` : list of files that should not be added to repository (data files, backup files, intermediate files). You can list one by one, the template or regular expressions (`*.csv` to ignore all files, `!dataset.csv` all except this one, # to make comments).

How do you connect your local and remote repository? SSH key! You first create a bridge `git remote add github_course git@github.com:jfaural/github_course.git`. Now things can go back and forth. You did not send anything yet. To send things through the bridge you use `git push` and the name of the repository. 

## Branches

It is useful for experimenting risk free, and also to collaborate in a project working in different tasks. Also you can look for different solutions on the same issue.

You create a branch with `git branch <name>`

WIth git checkout you can move from one branch to the other. You move through branches and commits.

# Thumb files

No one knows what a thumb file is. It is the great mystery of our time. Many have tried and failed to know it. In every folder, a thumb file may hide; luring, waiting, anticipating. Deep in the shadows of unpushed branches, between unsaved changes and lost files, it awaits its time to strike.
