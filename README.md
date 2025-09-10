# SE_project
Team project for NYU SE course Fall 2025

## Git Branches
For this project we will have
- main: The branch which will have every code that are implemented and tested.
- develop: The branch which will have every code you worked on the feature, and will be tested. The tested code will be merged to main from here.
- features: The feature branches are the ones we will implement each features at a time and will be merged to develop branch.

## Development Procedure
- Before starting to work on any code on your local branch, update your local develop branch up to date.
  git checkout develop
  git pull
- When you want to start working on a new feature, create a new local feature branch with the name "feature/..." from the develop branch.
  git checkout develop
  git checkout -b feature/...(The description of feature you will work) develop
- When you are done with working on the feature, push the local feature branch to remote repo, and make a pull request.
  git checkout ...(the name of the feature branch you worked)
  git status
  git add ...(file names you made change and want to apply to the remote repo)
  git commit -m "...Write a brief description of what have changed for implemented..."
  git push --set-upstream origin (the name of the feature branch)

  Go to the github repo online and check if your feature branch is there. If it is there and has all your changes, make a pull request to develop branch with code reivew.
- During the scrum meeting, we will do the code review for every pull request together and finally merge it to develop branch.
- Every 2 weeks, we will test the develop branch and if we all agree there is no other errors or edge cases, we will merge develop to main.
