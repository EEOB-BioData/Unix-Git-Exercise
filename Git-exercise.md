
### Roles of Git
1. Alerting Git to start tracking untracked files (this also stages the current version of the file to be included in the next commit.
2. Staging changes to an already tracked file (staged changes will be included in the next commit)

#### Staging files in Git: git add
To add any modification to `README` in the next commit, we stage them using git add and then we do git status **for example** 
`$ git add README`

`$ git status`

#### git commit: Taking a Snapshot of your Project
This command `git commit -m "initial commit (README.md)"` commits your staged changes to your repository with the commit message "initial commit README". 

Commit messages are notes to your collaborators about what a particular commit includes.

***
**Important**

We use the command `git commit -a or -m "your commit message"` The option `-a` or `-m` tells git to automatically stage all modified tracked files in this commit. Ideally commits should reflect helpful snapshots of your project's development, so including every every slightly changed file may later be confusing when you look at your repository history. Instead, make frequent commits that that correspond to discrete changes to your project like "**new counting  feature added**".

***
#### Seeing file differences: git diff
`git diff` shows you the difference between the files in your working directory and what has been staged. If none of your changes have been staged, `git diff`shows us the difference between your last commit and the current versions of your files.
**_Take Note_** 

`git diff's` output is easier to read as added lines will be **green** and deleted lines will be **red**
***

`git diff`
diff --git a/Markdown-hint/README.md b/Markdown-hint/README.md
index 4fd9efe..de8700e 100644


1.

`--- a/Markdown-hint/README.md`

`+++ b/Markdown-hint/README.md`

This line indicates that there are two versions of the README files we are comparing.
The `---` indicates the original file and `+++` indicates the changed version which we haven't commited. I edited the README file in `vi` but haven't staged/staged it yet.

2.



`@@ -1,2 +1,4 @@`

This denotes the start of a changed hunk and indicates which line the changes start on and how long they are.


3.

 `Notes from Chapter 05;Git for Scientists`
 
`+Helpful hints to work work with Git.`
+

Spaces before the line (e.g the line that begins Notes from Chapter 05) indicates nothing was changed.
The + sign indicates a line addition (the line that begins Helpful) and negative signs indicate a line deletion.
After we stage a file `git add`,`git diff` wont show any changes , because `git dii` compares the versions of files in your working directory to the last staged version **for example** 
`$ git add README`

`git diff` #shows nothing.
