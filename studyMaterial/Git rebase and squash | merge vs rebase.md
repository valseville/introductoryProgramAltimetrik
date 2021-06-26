# Git rebase and squash | merge vs rebase
Working with different branches, it comes the time when you need to take these changes to your master branch, and we have 3 different ways to do it, but this going to have repercussions in your way to work depending in what we choose. Due to the differents ways this works, this is a topic for discussion between developers. 

**Merge:** Incorporates changes from the named commits (since the time their histories diverged from the current branch) into the current branch. This command is used by ```$ git pull``` to incorporate changes from another repository and can be used by hand to merge changes from one branch into another. It’s the most common and safer way to do it, because it preserves all the history of branches and changes, it’s easier to go back to a commit, it looks like this

![](https://wac-cdn.atlassian.com/dam/jcr:4639eeb8-e417-434a-a3f8-a972277fc66a/02%20Merging%20main%20into%20the%20feature%20branh.svg?cdnVersion=1679)

**Rebase:** This operation works by going to the common ancestor of the two branches (the one you’re on and the one you’re rebasing onto), getting the diff introduced by each commit of the branch you’re on, saving those diffs to temporary files, resetting the current branch to the same commit as the branch you are rebasing onto, and finally applying each change in turn. The major benefit of rebasing is that you get a much cleaner project history. Re-writing project history can be potentially catastrophic for your collaboration workflow. And, less importantly, rebasing loses the context provided by a merge commit—you can’t see when upstream changes were incorporated into the feature.

Once you understand what rebasing is, the most important thing to learn is when not to do it. The golden rule of git rebase is to never use it on public branches.

![](https://wac-cdn.atlassian.com/dam/jcr:2908e0e6-f74b-4425-b5d2-f5eca8cfcd99/05%20Rebasing%20the%20main%20branch.svg?cdnVersion=1679)

The rebase moves all of the commits in main onto the tip of feature. The problem is that this only happened in your repository. All of the other developers are still working with the original main. Since rebasing results in brand new commits, Git will think that your main branch’s history has diverged from everybody else’s.

```$ git rebase master server```


**Squash:** Compact all the commits in this request into one (rarely to other number) to make it more concise, readable and not to pollute main branch’s history. To achieve this, a developer needs to use interactive mode of Git Rebase command.
Quite often when you develop some new feature you end up with several intermittent commits in your history - you develop incrementally after all. That might be just some typos or steps to final solution. Most of the time there is no use in having all these commits in the final public version of your code, so it’s more beneficial to have all of them compacted into one, single and final version. This one have the other problem like rebase doesn’t preserve the history it’s pretty destructive and you can’t go back.

![](https://i.postimg.cc/fRW4Wsjc/Screen-Shot-2021-06-26-at-18-24-59.png)

```$ git merge --squash feature/login```

Links

- https://www.youtube.com/watch?v=7Mh259hfxJg
- https://www.youtube.com/watch?v=RwvTrSm7zEY
- https://www.youtube.com/watch?v=RwvTrSm7zEY
- https://www.git-tower.com/learn/git/faq/git-squash/
- https://www.freecodecamp.org/news/git-squash-explained/
- http://blog.nerdbank.net/2020/01/should-i-merge-or-rebase-in-git.html
- https://www.perforce.com/blog/vcs/git-rebase-vs-merge-which-better#Git%20Merge
- https://git-scm.com/docs/merge-options
- https://git-scm.com/book/en/v2/Git-Branching-Rebasing
- https://www.atlassian.com/git/tutorials/merging-vs-rebasing
- https://www.freecodecamp.org/news/git-squash-explained/