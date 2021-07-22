## Git ##

Git --fast-version-control
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.

## Branch
A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process. You can think of them as a way to request a brand new working directory, staging area, and project history. New commits are recorded in the history for the current branch, which results in a fork in the history of the project.

## Fork
Instead of using a single server-side repository to act as the “central” codebase, forking gives every developer a server-side repository. This means that each contributor has not one, but two Git repositories: a private local one and a public server-side one.

## HEAD
Git’s way of referring to the current snapshot. Internally, the git checkout command simply updates the HEAD to point to either the specified branch or commit. When it points to a branch, Git doesn't complain, but when you check out a commit, it switches into a “detached HEAD” state.

## Master
The default development branch. Whenever you create a git repository, a branch named "master" is created, and becomes the active branch.

## Pipelines
Bitbucket Pipelines is an integrated CI/CD service, built into Bitbucket. It allows you to automatically build, test and even deploy your code, based on a configuration file in your repository. 

## Pipes
Bitbucket Pipes are short code chunks that you can drop into your pipeline to perform powerful actions. Pipes make it easier to build powerful, automated CI/CD workflows and get up and running quickly.

## Project
A project is a container for repositories. Projects make it easier for teams to focus on a goal, product, or process by organizing your repositories into projects. Projects can be either visible or hidden from public view.

## Pull Request
Pull requests are a feature that makes it easier for developers to collaborate using Bitbucket. They provide a user-friendly web interface for discussing proposed changes before integrating them into the official project.

## Working Tree
The tree of actual checked out files, normally containing the contents of the HEAD commit's tree and any local changes you've made but haven't yet committed.



