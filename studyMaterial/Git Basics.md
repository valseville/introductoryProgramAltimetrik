# Git Basics

## What is version control software?

We can say that git is a content tracker. Developers can work the same code in parallel, git save the history of the changes by the day, time, person, and the changes added or deleted. Also, offer a remote distribution repository (Github the most common service used) that helps with the collaboration work and save the code in a **“master branch”** so it’s easier to share the work or review it with other developers

**Git branch:**  Branches are spaces or enviroments for developers to use it, in this way they can work in change without changing the original one.

**Tags:** The tags in git and github are tag for save an specific version or release of the code and remains the same even when we push more code

```$ git tag -a v1.4 -m "my version 1.4" ```

 **Commit:** This is a command that saves the changes you did in your local repository before you pull out to master, basicly creates a snapshoot of your work, another version

```git commit```
```git commit -am “message”```
```git commit -m “mesagge”```

**Stash:** This is a command that makes a quick saves a file of what you are working on, but reset the code to the last commit

``` git stash ```

**Hooks:** Are scripts that runs when you execute specifics commands

 ``` post-commit ```
``` post-checkout```
```post-merge```
```post-rewrite```

### Basic git commands

```Git init```
```Git diff```
```Git commit -am “message”```
```Git commit -m```
```Git push```
```Git pull```
```Git checkout -v name```
```Git checkout ```
```Git clone ```
```Git add ```
```Git rm ```
```Git rm -rf ```
```Git rm -f ```
```Git log ```
```Git status ```
```Git reset —hard```

