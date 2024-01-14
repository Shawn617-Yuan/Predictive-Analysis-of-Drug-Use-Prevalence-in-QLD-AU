# Understand the environment and factors in which drug use is prevalent in Queensland

## Project Overview:
This project aims to understand the environmental and social factors contributing to drug use prevalence in Queensland. Using open crime data and census reports, the research explores correlations between drug use and various societal factors.

## Data Sources:
**Queensland LGA Vector Dataset:** Geographic information on Queensland Local Government Areas.
**Queensland LGA Crime Rate Dataset:** Crime rates per capita across different LGAs from 2001 to 2021.
**Australian Census Dataset (2016):** Population demographics and education levels, aggregated by LGA.

## Methodology:
- Data preprocessing involved merging datasets and standardizing location names for compatibility.  
- Focused on understanding the relationship between drug offences and factors such as crime types, age groups, and education levels.
  
Conducted regression analysis using the following models to identify the best-fitting model based on the mean squared error:
1. Linear Regression  
2. Lasso Regression (use 10-fold cross validation to find lambda parameter)  
3. Ridge Regression (use 10-fold cross validation to find lambda parameter)  
4. Poisson Regression (since the target is a count of incidences and may be Poisson distributed)

## Key Insights:
- Found strong correlations between drug offences and specific crimes like handling of stolen goods and liquor offences.
- Identified demographic trends indicating higher drug use prevalence in areas with younger children and less educated individuals.
- Highlighted the need for targeted law enforcement and educational strategies to address drug use in affected communities.

## Recommendations:
- Law enforcement agencies should focus on areas with a higher prevalence of specific crimes strongly correlated with drug use.
- Develop targeted anti-drug education and community support initiatives, especially in communities with vulnerable demographics.
- Policymakers should consider the insights from this analysis to inform more effective drug prevention and intervention strategies.

## Future Work:
- Extend the scope of the study to include more recent data and additional variables.
- Explore the effectiveness of existing anti-drug policies and community programs on reducing drug-related offences.

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
