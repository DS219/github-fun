## Making changes
### Step 2.1 Creating a file
Create a file called `question.txt` in your new repo (inside the folder you downloaded with `git clone`) and add the question “What makes you excited about programming?” (Or add your own question!) Feel free to do this however you are most comfortable creating and editing files (MS Word is fine), but please save it as a `.txt` file instead of `.doc` or any other file extension.

### Step 2.2 Tracking changes
Check the status of your new file with:  
`git status`  

You should see something like:  

```
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	question.txt

nothing added to commit but untracked files present (use "git add" to track)

```


Add the file to git's tracking with:  
`git add question.txt`

Use `git status` to check the status of your file again. What is different? Now you should see something like:  
```
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   question.txt
```

### Step 2.3 Committing changes

To commit your changes and create a save point, use:

`git commit -am "added question.txt file"`  

Tip: `-m ` allows you to specify a commit message. The commit message should be short and descriptive about the purpose of the commit or what you changed in the repo. `-a` creates a snapshot of all changes to tracked files in the working directory.

You should see:
```
[master 41e204c] added question.txt file
 1 file changed, 1 insertion(+)
 create mode 100644 question.txt
```

### Step 2.4 Storing changes remotely
To see which remote branches your branch is tracking, use:  
`git remote -v` 

You should see something like:
```
origin	git@github.com:<gitusername>/<repo>.git (fetch)
origin	git@github.com:<gitusername>/<repo>.git (push)

```

Then to push your committed changes from your local machine to the remote GitHub repo, where others can see it or clone it, use:  
`git push origin master` 

You should see:  
```
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 330 bytes | 330.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:<gitusername>/<repo>.git
   9e62e6c..41e204c  master -> master

```
