# Git & Github Cheatsheet

## Git vs Github

-   You can think of Git as the method of transportation used to transport your code and github as the online location it is stored. e.g. git is the uhaul truck and github is the storage locker.

## Repository

-   A repository is a location in which all of you code lives. You can have as many of these as you'd like.

-   A repo (short for repository) can be public or private. A public repository is one that anyone can view the code and clone (download) A private repo is one that only you and those you invite to can see and clone.

## Branches

-   A repo can have multiple branches. They are like individual sandboxed versions of your code. When you create a new branch it is created as a copy of main (used to be called master a while back)

-   Popular use cases of branches are to separate developers, so that each developer can build their code out in their own sandboxed version of the project without fear of messing up the other developers code. Additionally it can cut down on merge conflicts with everyone working in their own sandbox and making pull requests to pull their finalized changes into main (master) Another popular use case is for feature sets, if you have a working code base on the main branch that you don't want to mess up you can create a new branch which will make a copy main do your "scratch work" so to speak and then when finalized open a pull request to pull in the new feature you developed on your new branch into main.

## Forks

-   Forks are a means of copying a repo that belongs to another user. It creates a new copy of that repo under your account which you can then push & pull to you hearts content

## Cloning

-   This is just nerd speak for download, you can simply clone a repo by clicking the green code button in the top left of the repo and copying the https address listed. You can then run "git clone < address you copied goes here >" and it will download the repo to wherever your current terminal's path is pointed at.

## Pushing

-   You can use this to update the repo in github. If you have changes on your local machine that are NOT on your github repo you can simply run the three commands listed below to push your code.
    -   git add .
        -   You can push only certain files by listing them out w/ their extension separated by spaces
        -   . will stage all files that are not located in the repo and any files that have changes that are different than from what exists in the repo
    -   git commit -m '< your commit message here>'
    -   git push

## Pulling

-   Pulling is used to pull in changes that exist on github but NOT on your local machine, e.g. github has a file on it that I do not have on my computer. To fix this I would use "git pull"

-   You will not be able to push code if your local machine does not have the latest commit in github, rule of thumb before you write any code go ahead and run a git pull to make sure you have everything you need as untangling this can be a bit messy.

## Pull Requests

-   A pull request is a request to pull in code from one branch to another branch, or from one fork to another. To make things even more messy it is even possible to open pull requests between forks over two different branches though this shouldn't happen often.

-   Pull requests are done on github through the web application, they can be done in the terminal but its highly recommended you open/close pull requests on the github website as you are far less prone to cause errors.
    -   There are two actions involved with a pull request, opening the request & closing the request.
        -   Opening the request is done by clicking pull requests in the top navigation of the repo. Clicking the green create new pull request button. You will have two drop downs with an arrow between them. The one of the left is branch/fork that will have the changes merged into. The one on right is the branch/fork in which the changes are coming from. You will then be prompted to leave a comment and congrats you've opened a pull request.
            -Closing a pull request starts the same way by clicking pull request in the op navigation of the repo. You will be presented with a list of open pull requests if there are any open. Click the pull request you'd like to close. You will then either have a button that says close pull request in green (yay!) or a red/grey button that denotes that there are merge conflicts that must be resolved before the branchs/forks can be merged.

## Gitignore

-   this file is ".gitignore" in here you can place files or directories that you want git to NOT push to github. You can denote a file that you do not want to be sent with "filename.ext" and directories with "/directoryName"

## Git branch

-   will list all the available (visited) branches for the repo you are currently located in. The one you are currently on will be denoted with an "\*"

-   you can also create a new branch like "git branch < branch name >"

## Git checkout

-   git checkout can be used to switch between branches. e.g. "git checkout < branch name >"

