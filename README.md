# CSCI 432 Fall 2023 Repo for LaTex Files

## Creating Your Own Repository 

The repository is set as public, so you can access all course materials easily.
I suggest creating a private repository with this one setup as an upstream git
repo, so that you can use your repository to maintain your own materials for
this class. 

To do so, follow these instructions:
    
    - Going to <https://github.com/new>
    - Enter the name `csci-432-fall2023-yourname`
    - Select `Private`
    - **DO NOT ADD A README.MD or .gitignore!**

Once your repository is initialized, you can pull it down to your local machine.

Next, you should add the class repository as an upstream git repo:

```bash
$ cd csci-432-fall2023-yourname
$ git remote add upstream https://github.com/msu/csci-432-fall2023-latex.git
$ git pull upstream main
$ git push
```
This will synchronize your private repository with the class repository.  You
only need to run these commands once.  Then, when you want to get an update from
the public class repository you can run this command:

```
$ git pull upstream main
```

As a general workflow on your own repository, I suggest:
```
$ git pull upstream master
[[ do work here ]]
$ git add [[ list filenames edited ]]
$ git commit -m "Descriptive message here"
$ git push origin main
```

