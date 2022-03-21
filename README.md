# Template Repository

## Git 
### Tutorial links
* [Tutorials Point's Git Tutorial](https://www.tutorialspoint.com/git/index.htm)
* [BitBucket's Git Tutorial](https://www.atlassian.com/git/tutorials)


### Read more about using Github to manage Git:  
[Getting Started with Github](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github)

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
4. You can visually manage branching, pull requests, and hosting sites / apps on GitHub. 
* Get Github Desktop to easily manage your repositories: [Download it Here](https://desktop.github.com/)
* Hosting HTML files on your own statis site on GitHub: [Website Hosting](https://pages.github.com/)

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

