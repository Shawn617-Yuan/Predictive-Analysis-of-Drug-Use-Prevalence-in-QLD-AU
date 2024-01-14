# Understand the environment and factors in which drug use is prevalent in Queensland

We have two datasets to work on ... the crime data by itself over time and the merged census data, which is aggregated to only include one observation per LGA in 2016. For each of these datasets, we want to fit the following models ...
- Linear Regression [Fred]
- Lasso Regression (use 10-fold cross validation to find lambda parameter) [Paff]
- Ridge Regression (use 10-fold cross validation to find lambda parameter) [James]
- Poisson Regression (since the target is a count of incidences and may be Poisson distributed) [Shawn]
- Any other models?

y_pred = b0 + b1 x1 + b2 x2 + ....
mse = sum((y_pred - y_actual)**2) # lowest mse

- Poisson is difficult to do, but when done crudely it underperforms linear, so choose linear regression

## Group project Git Repository

I think this will be a great place to coordinate our project, and great for the resume later on ;)

## Google Drive
All the Google Docs and meeting recordings are in the drive  
[Link to the Google Drive](https://drive.google.com/drive/folders/1KvkitYDhhV8dDvRbm5zG50Ls9K-Xo2dA?usp=sharing)  
[Link to Presentation](https://docs.google.com/presentation/d/1_wFsb38l6narmrn_Bi5KJJtAfITm1tTUyJ7W4bo_HZA/edit?usp=sharing)

## Git Tutorials

[Atlassian Cheat Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

[Atlassian Tutorial](https://www.atlassian.com/git/tutorials)

## Git quickstart tutorial
So this is just some basic instructions to get started with putting the development environment on your computer. 
1. Create a directory to work in
2. Open the git command line and cd into that directory
3. Type `git init` to initialise this directory as a git directory
4. We now want to connect this directory with github
  - type `git remote add origin <url>`
  - The url can be found by clicking the green code tab on the github website
  - This links the directory with the github repo, which will be called "origin"
5. Now, we want to set up the folder so that it is linked with GitHub
  - Pull the repository down `git pull origin main`
  - Create new branch main `git branch main`
  - Switch over to that branch `git switch main`
  - Link this branch with github `git branch --set-upstream-to=origin/main main`
7. Now to download the latest version of the repository, we want to pull it
  - type `git pull`
  - it should prompt you for your username and password
8. If all went well, then you should see this readme file and any other documents we have saved in your working directory

## Git workflow
While working on the project, you should follow the basic steps outlined here
1. When starting a session, pull down the updates with `gut pull`
2. While working, you can save your progress using the following steps
  - Add work to staging area `git add <filenames>` (to add all files, just use `git add .`)
  - Commit the work to the repo `git commit -m "Enter your commit message here"`
    - Your commit message should be a one-liner about what you changed/did
  - Save your work often, ideally every time you finish a task
3. When you want to submit the work back to github, use `git push`

### Hint
If git keeps asking for a username and password, you can cash them by typing 
`git config credential.helper store`
The next time you put in your username and password it will remember them
