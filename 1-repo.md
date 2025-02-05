## Creating a repo
### Step 1.1 Creating a repo on GitHub
In your GitHub account, find the Repositories tab and click. Then click the green New button.

![PACSPull Plugin](/images/repo/github-new-repo.png)

Choose a name for your repo (ex. `myawesomerepo`). Choose the button to make the repo public and select “Initialize this repository with a README.” Leave all other choices on the default setting.

![PACSPull Plugin](/images/repo/github-repo-initialize.png)

### Step 1.2 Cloning the repo locally
Copy the repo's URL. In your GitHub account, click the Repositories tab and click on your new repo. Click the green “code” button on the right. Make sure "SSH" is selected.

![PACSPull Plugin](/images/repo/github-clone-repo.png)

In the terminal, navigate to your home directory and create a github directory:

Note: this step is not needed, but it will help us keep all our github repos under one location so it is easy for us to find in the future.
```
cd ~
mkdir github
```

Then navigate to the github directory and clone your repo there:
```
cd github
git clone <URL>
```

You should see something like this:
```
Cloning into 'myawesomerepo'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
```

Then change directory to your local repo with:
```
cd myawesomerepo/
```

Now you are inside the repo folder. You can see the files in your repo by using:  
`ls`

This should show you:  
`README.md`
