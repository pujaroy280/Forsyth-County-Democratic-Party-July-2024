# Template Repository

## Git 
[Tutorials Point's Git Tutorial](https://www.tutorialspoint.com/git/index.htm)
[BitBucket's Git Tutorial](https://www.atlassian.com/git/tutorials)

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

## Data Guide 

[Data Guide Documentation Here](https://docs.google.com/document/d/117OsHl77wyzDyEItQyr4ZmmwDtHCsW6pukC63mXut2w/edit)

## R Docs
[coming soon]
## Python Docs
[coming soon]
## VAN Docs
[VAN/Data Slides](https://docs.google.com/presentation/d/1yuEKgZQAlnpWOLEpBtRPCba4QyelkvfX1nuhnCiEjW8/edit)

## [New Fellows Training Guide Easy Access](https://docs.google.com/document/d/1c0BH66W-C0BJB-yrPQ3740neOrswRrdO1iJbUaCedqw/edit)
