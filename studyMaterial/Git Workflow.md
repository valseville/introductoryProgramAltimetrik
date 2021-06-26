
- # Git Workflow

  The git workflow is called Gitflow and consists of how the developer works with the different branches, the branches are spaces or environments where you can code and you can create as many as you need.

  The branches defined in this workflow are:

  ![](https://david-estevez.gitbooks.io/the-git-the-bad-and-the-ugly/content/assets/gitflow.svg)

  **Master**  - Its the main branch, the one that is in production, and the users interact with

  **Develop** - It’s a copy of the main branch but it’s a safe space to test releases and features

  **Releases** - The purpose of this is to prepare to develop to merge with master

  **Features** - This branch is for features and can be as small or big as needed

  **Hotfix** -  This branch is for bug fixes that merge directly to master and develop 


  Github complements this workflow with features like “Pull request”, which enables other developers to check the code before merging to master. You can add comments, approve, deny or ask for changes. GitHub has a history of all of these activities. Github understands tags, saves and preserve all the versions


  - https://www.youtube.com/watch?v=aJnFGMclhU8
  - http://book.git-scm.com/book/en/v2/Git-Branching-Branching-Workflows
  - https://www.youtube.com/watch?v=Lj_jAFwofLs
  - https://www.youtube.com/watch?v=1SXpE08hvGs