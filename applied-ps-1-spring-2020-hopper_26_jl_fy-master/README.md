This is the starter repo for 30535 Data and Programming for Public Policy I. This README includes 
1. An explanation of the problem set front matter
1. An outline of the homework workflow
1. An overview of Git and Github.

# Problem Set Front Matter
1. Problem sets are due at 5 pm on Friday. You have 4 late coins for the quarter. A late coin extends your deadline 24 hours. You may use up to 2 on a given problem set. When you are using late coins please acknowledge this in the front matter of your problem set.
1. For each problem set, you will acknowledge that you are following the integrity policy. Please list all classmates who you consult with on a given problem set. 

# Problem Set Workflow (see video for more details)
1. Go to the assignment invitation url in the problem set, and accept the invitation.
1. This forks (copies) the starter repository into our organization's repository (datasci-harris), with your Github username.
1. Click the link where the assignment repository was created, and clone this remote repository to your local computer using GitHub Desktop. Do this by clicking Set up in Desktop. Make sure to choose the local folder you would like to clone the repository into. GitHub Desktop will default to the last folder you have used.
1. Rename `pset_template.Rmd` as directed by the homework. Complete the assignment within this renamed file.
1. Delete the `pset_template.html` file from your repository. It only exists as an example.
1. Use `knitr` to create an html document of your assignment. It should have the same name as the `.Rmd` file, but with a `.html` extension.
1. Commit and push your finished assignment to Github using GitHub Desktop.

Note: The html files can be viewed in a web browser (e.g. Firefox).  GitHub does not automatically render html documents, so you will not be able to preview them easily on Github.

# GitHub Desktop and GitHub

Throughout the course you will use GitHub Desktop to submit homework. To see detailed videos with an introduction to using Git for this class, see [these videos](https://canvas.uchicago.edu/courses/28237/files/folder/Videos/git%20primer) on canvas.

GitHub provides online storage with version control using software called `git`. Everytime you commit a change, `git` tracks those changes. This is useful when you want to go back to look at old work without storing multiple copies of a file and also allows for sophisticated collaboration on shared files.


## Overview

You will use GitHub Desktop to add files, commit, and push them to your remote repository. You can also use GitHub Desktop to remove files and undo changes/revert to an older version.




## Explanation

For the purposes of this class, we will only use a few of the many available `git` commands:

### clone
`git clone` creates a copy of a local or GitHub repository (repo). By cloning a repo, we can download files from GitHub, make changes locally, and then push those changes back to GitHub to make them available to others. Cloning a GitHub repo will also set that repo as the default remote repo (the default location to push to). To clone from GitHub to your local computer using GitHub Desktop, go to a repository on Github and click Clone or download, and Open in Desktop.

Choose the local folder you would like to download the repository into.

### commit
Once you've added files or changes to your local repository, you need to commit them. Committing is a way to take a snapshot of the state of your files, i.e. *commit* your changes to `git`'s memory. Each commit represents your files at a specific point in time, and you can jump back to any one of those points without losing data. You must commit before pushing to GitHub. To commit files or changes inside files, go to GitHub Desktop, and in the bottom right of your window, type a meaningful commit message and press `Commit to master`. The commit message is something describing the changes you've made. Most first time commits use the message `Initial commit`.

### push
After committing your changes, you can now push your commit to GitHub. If you've cloned a GitHub repo, `git` will push back to that repo by default. Simply press "Push Origin" either at the top or in the middle of your window.

This will push any files or changes you've made to the remote repository, in this case GitHub, where you can view them online.

### pull
If you want to retrieve changes made to a remote repository, such as one on GitHub, you can pull them to your local repository. Pulling will download changes to your local repository. Assuming you are working in your current repository in GitHub Desktop, you can press Fetch origin at the top of the window. If there were changes made to the remote repository, the button will change to Pull Origin. After you click Pull Origin, your local repository will reflect the changes made in the remote.

Note that if you have unadded/unindexed changes in your files, git pull will overwrite them.

### Using .gitignore
By default, GitHub Desktop tracks all files within your local repository. Sometimes this is inconvenient, such as when working with large CSV files that don't need to be tracked or on GitHub. In this case you can use the gitignore feature to instruct git not to track these files.

To do this, go to GitHub Desktop, and click Repository > Repository Settings on the toolbar. Doing so opens a small window that allows you to specify which files or types of files to ignore. For example, if one wants to ignore all CSVs, then add the line `*.csv`. This will ignore all files with the extension `.csv`.


