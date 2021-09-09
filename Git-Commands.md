```diff
- Just for private purposes!!!
```

# commands
* ## git init
  * **This command turns a directory into an empty Git repository. This is the first step in creating a repository. After running git init, adding and committing files/directories is possible.**

### Usage:

```diff
# change directory to codebase
$ cd /file/path/to/code

# make directory a git repository
$ git init
```

### In Practice:

```diff
# change directory to codebase
$ cd /Users/computer-name/Documents/website

# make directory a git repository
$ git init
Initialized empty Git repository in /Users/computer-name/Documents/website/.git/
```
&nbsp;


* ## git add
    * **Adds files in the to the staging area for Git. Before a file is available to commit to a repository, the file needs to be added to the Git index (staging area). There are a few different ways to use git add, by adding entire directories, specific files, or all unstaged files.**

### Usage:

```diff
$ git add <file or directory name>
```

### In Practice:

```diff

# To add all files not staged:
$ git add .

# To stage a specific file:
$ git add index.html

# To stage an entire directory:
$ git add css
```
&nbsp;


* ## git commit
    * **Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID.**

    * **It’s best practice to include a message with each commit explaining the changes made in a commit. Adding a commit message helps to find a particular change or understanding the changes.**
    
### Usage:

```diff
# Adding a commit with message
$ git commit -m "Commit message in quotes"
```

### In Practice:

```diff
+ If You give This Command:
$ git commit -m "My first commit message"



+IZ SHOWS YOU: 
[SecretTesting 0254c3d] My first commit message
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 homepage/index.html
```

* ## git status
    * **This command returns the current state of the repository.**
**git status will return the current working branch. If a file is in the staging area, but not committed, it shows with git status. Or, if there are no changes it’ll return nothing to commit, working directory clean.**

### Usage:

```diff
$ git status
```

### In Practice:

```diff
# Message when files have not been staged (git add)
$ git status
On branch SecretTesting
Untracked files:
  (use "git add <file>..." to include in what will be committed)

  	homepage/index.html

# Message when files have been not been committed (git commit)
$ git status
On branch SecretTesting
Your branch is up-to-date with 'origin/SecretTesting'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   homepage/index.html

# Message when all files have been staged and committed 
$ git status
On branch SecretTesting
nothing to commit, working directory clean
```