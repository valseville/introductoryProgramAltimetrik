# Git Basics

## What is version control software?

We can say that git is a content tracker. Developers can work the same code in parallel, git save the history of the changes by the day, time, person, and the changes added or deleted. Also, offer a remote distribution repository (Github the most common service used) that helps with the collaboration work and save the code in a **“master branch”** so it’s easier to share the work or review it with other developers

**Git branch:**  Branches are spaces or environments for developers to use, in this way they can work in change without changing the original one.

``` $ git checkout ``` 

**Tags:** The tags in git and GitHub are tag for save a specific version or release of the code and remains the same even when we push more code

``` $ git tag -a v1.4 -m "my version 1.4" ```

**Commit:** This is a command that saves the changes you did in your local repository before you pull out to master, basically creates a snapshot of your work, another version

``` $ git commit -m “message” ```

**Stash:** This is a command that makes a quick saves a file of what you are working on, but reset the code to the last commit

``` $ git stash ```

**Hooks:** Are scripts that run when you execute specifics commands

``` $ post-commit ```
``` $ post-checkout```
``` $ post-merge ```
```$ post-rewrite ```

```$ pre-commit```

```$ pre-push```



## Basic git commands

Creates a new repository
```$ git init```

Verify changes in the repository
```$ git diff```

Saves and adds changes automatically (you can add a description of the change)
```$ git commit -am “message”```

Saves changes (you can add a description of the change)
```$ git commit -m```

Upload the local repository to remote
```$ git push```

Download the local repository to remote 
```$ git pull```

Change between branches but if the “name” doesn’t exist creates a new one with the “name”
```$ git checkout -b name```

Change between branches
```$ git checkout name ```

Clone a remote repository to local 
```$ git clone remote-location```

Add the files with changes
```$ git add file```

Untrack a file
```$ git rm```

History of the repository
```$ git log```

Get current repository status
```$ git status```

Delete all changes and restore to the last commit
```$ git reset —hard ```

### Links Git
- https://www.gitkraken.com/learn/git/commit#:~:text=In%20Git%2C%20a%20commit%20is,reflected%20in%20your%20Git%20repository.
- https://www.freecodecamp.org/news/what-is-git-learn-git-version-control/
- https://www.nobledesktop.com/learn/git/what-is-git
- https://git-scm.com/
