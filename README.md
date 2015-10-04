# gdg_OSource_prep

## Lets start with Git

###*What is Git?*
In strict terms, Git is a "distributed version control management system".
In simpler terms, Git is a "source code management system". It allows a team/group to work on projects, and the same pieces of code. More importantly, it helps them avoid the confusion which would normally arise with multiple people editing the same files simultaneously.
You will get the gist of it in time with experience. This git tutorial is aimed at getting you started with the basics. You aren't expected, or required, to understand the details all at once. But you are expected to follow along. *And ideally, experiment with and read up about git once you'r done here.*

###*Join Github*

*Github IS NOT git!* More about that and what github is later.
Create your github account for now: https://github.com/join

###*Setting up git*

**If on Windows**, you can use the git command prompt as well as the git for windows GUI (Graphical User Interface). The choice is upto you but the command line method is recommended. 
Check out the following link for more: [Installing on Windows](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git#Installing-on-Windows)

**If on Linux**, use the terminal. Install/upgrade git on your system.
```
# Install git (on Ubuntu)
sudo apt-get install git
# Install git (on Fedora)
sudo yum install git
```

**Further instructions assume that the user is using the command line method.**

###*Cloning a repository*

The ```git clone``` command does exactly what it sounds like. It lets you create a copy (clone) of an existing git repository.
For starters, clone this very repository on your local machine:
```
git clone https://github.com/da-ta-vinci21/gdg_OSource_prep.git
```

Check the contents to make sure it worked:
```
cd gdg_OSource_prep.git
ls
```

###*Checking status and Making changes*

Check the current status of the git repository you just cloned:
```
git status
```
Nothing to be done as of now.

Open the tutorial markdown file using an editor of your choice.
To open it via terminal in an editor like gedit:
```
gedit README.md
```

Make some changes in the README file and save it. Anything at all!

Now, check the status of the repository again.
It should show a message like this:
```
Changes to be committed:
README.md
```

Now we head to the most awaited parts.
*Drumrolls*

###*Adding and Committing changes*

You have made the changes. Now you need to share them. But how do you do that?
A commit is like taking the snapshot of a git repository's contents at a particular moment and storing them. In the background, git only stores the changes made since the last commit. That's what the earlier status message had hinted at.

But first you will have to add the pending changes to the git's staging area. For now, just do this without bothering about the details. (Read reference [] for more)
```
git add .
```

Okay then, time to make the commit:
```
git commit -m "First commit"
```

The snapshots are always committed to the *local* repository. That brings us to yet another important aspect of git.

###*Remotes*
