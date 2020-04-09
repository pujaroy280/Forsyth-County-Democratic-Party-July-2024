# Template Repository

## Git 
### Tutorial links
* [Tutorials Point's Git Tutorial](https://www.tutorialspoint.com/git/index.htm)
* [BitBucket's Git Tutorial](https://www.atlassian.com/git/tutorials)

### General Git primer
* Here are the main commands you'll probably be using when you start off: 
```
git clone [repository link here]
git pull 
git add . 
git commit -m "[enter message]"
(or git commit -am "" to combine git add . and git commit -m together)
git push 

```

* Git collaboration tips: 

1. This is something that will need to be discussed amongst your team members. 
2. If you'll be starting off working in completely separate files, then perhaps using one master branch to collaborate makes the most sense. 
3. However, if you're working on an intertwined project where everyone might be touching the same file at some point, perhaps isolate your own work on your own branch and have an updated master branch where you can pull from for updates from other members. This keeps the work more clean and easier to figure out what code needs to be focused on if there are conflicts and/or errors. 

## Git Repo Managers ++  
On Gitlab, just like on more well known repo managers like Github, we can fork a template repository for each campaign team and make it a private repository within each campaign team's Bluebonnet Sub-Group.

1. You may have some SSH keys left over from Github authentication. To make authentication for Gitlab smoother, follow these steps: [Gitlab SSH Auth](https://docs.gitlab.com/ee/ssh/)
2. To start working with your campaign's repository, make sure you clone this locally. You should have permissions to clone this and contribute now after the SSH keys (or if you skipped that step, perhaps just entering manually the authentication when prompted by the terminal after running the git clone command)
3. Once you have your ssh keys set based on step 1, make sure you git clone from the ssh route. However, if you're not setting up ssh keys and you're cloning from http instead, you would set up the following: 
4. When cloning a private repository, you'll need to use a personal token for cloning HTTP: Go to [your personal access tokens](https://gitlab.com/profile/personal_access_tokens) > Name the token > Check off `read_repository` and `write_repository` > Press the 'create personal access token' button > make sure you save that token somewhere 
5. Enter the following in the terminal to clone: git clone https://<YOUR USERNAME>:<YOUR PERSONAL ACCESS TOKEN>@gitlab.com/<GIT REPOSITORY PATH>
6. Besides all of the above, you should be able to also download the zip file version. 
7. When you download the zip file version, you would need to follow these terminal commands: 
```
cd <your cloned repo name> 
git init 
git remote add origin git@gitlab.com:<enter repository path here>
git pull origin master --allow-unrelated-histories (assuming you didn't make any changes) 
git add . 
git commit -m "<your commit message>"
git push --set-upstream origin master 
```

```
git clone https://gitlab.com/bluebonnet-data/[replace with campaign team's respository name here].git
```

3. Test trial run with Git (Gitlab-independent exercise) Feel free to add a random file (if you add a directory, make sure it has .gitkeep as a file in there so it shows up) 
```
git pull /* to make sure everything in your directory is updated and there won't be conflicts */
git add . 
git commit -m "adding my first random file!"
(or git commit -am "" to combine git add . and git commit -m together)
git push 
```

4. You can visually manage branching, pull requests, and hosting sites / apps on GitLab. [more to be added about this soon]
*  Hosting HTML File on Gitlab: [Website Hosting](https://gitlab.com/bluebonnet-data/collab-test/bluebonnet-data-website-hosting-template)

## Trouble shooting above steps (you're not alone)
When cloning a private repository: 
```
remote: HTTP Basic: Access denied
```
* https://gitlab.com/gitlab-org/gitlab-foss/-/issues/30275
* https://gitlab.com/gitlab-com/support-forum/issues/2869
There are a couple of ways people have resolved the issue via terminal. The key point is that you have to authenticate or trigger authentication (log in / verify you're able to clone a private repository)
The above steps to put your username and personal access token is pretty straightforward. Otherwise you can also follow the steps they have in those links. 

## [Data Guide Documentation Here](https://docs.google.com/document/d/117OsHl77wyzDyEItQyr4ZmmwDtHCsW6pukC63mXut2w/edit)

## R Docs
[coming soon]
## Python Docs
[coming soon]
## [VAN/Data Slides](https://docs.google.com/presentation/d/1yuEKgZQAlnpWOLEpBtRPCba4QyelkvfX1nuhnCiEjW8/edit)

## [New Fellows Training Guide Easy Access](https://docs.google.com/document/d/1c0BH66W-C0BJB-yrPQ3740neOrswRrdO1iJbUaCedqw/edit)

## Repository File Structure: [Click here for CookieCutter Datascience's Breakdown](https://drivendata.github.io/cookiecutter-data-science/)

```
├── README.md          <- The top-level README for developers using this project.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── data
│   ├── processed      <- The final, canonical data sets for modeling.
│   │
│   └── raw            <- The original, immutable data dump.
│
├── src                <- Source code for use in this project.
│   │
│   ├── production     <- Final, working code
│   │   
│   └── testing        <- Code that is in development
│   
└── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │
    └── figures        <- Generated graphics and figures to be used in reporting
```
