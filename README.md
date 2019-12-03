# GitHub Tutorial

_by Ryan Chen_

---
## Git vs. GitHub

_What is the Git and Github?_

> Git and GitHub are separate from one another even though they are used together. They may have the word "Git" but they function completely different from one another. Git acts more like a tool that keeps track of the changes you make while you're programming where you're able to look back what you've done. On the other hand, Github is used is a server that stores all your information digitally so you can access it anywhere rather than locally where it only available in your laptop/device.

Git | GitHub
---|---
Access Locally | Access Globally
Doesn't requires wifi | Requires wifi
It's on your computer | Collaboration with other

_What is a repo? Local vs Global?_

> Repo is a short acronym for a repository, but you would wonder what is a repo and what does it do. A repository is a place where information can be stored and can be accessed later on. In this case, a repo is stored in GitHub where your project can be accessed anywhere with connection with wifi. This leads up to the questions what the difference between a local repo and a global repo. A local repo can only be accessible within the device that you store the information in and in order to share it you either have to store it within a server, but with a global repo, you can store it and access it in a different computer that isn't you own which is convenient.


---
## Initial Setup

### Step 0: Get a github account

Create a github account [here](http://github.com) (accounts are free) then go to [IDECS50](ide.cs50.io) and login with your github account

Follow the steps [here](https://github.com/hstatsep/ide50) to set up your IDECS50

### Whats is SSH?

> SSH stands for Secure SHell which goes through a protocal to help someone safety access the net.

---
## Repository Setup

Before anything, you need to initialize your git, create a directory that your file will be contain at by using `Mkdir < File Name >`. A directory is a library that stores your information or project within such as files, documents, images, and videos. After you initialize your git you would need to `cd < file name >` to make any changes within the directory. Then you would need to do `git init` to initialize the git which makes the file into the parent function of every other. This also means that you can store anything within where it's considered as the `(master)` in your code.

As you start making changes to your files start checking what you have done by using `git status` to see the changes that you're making before you're committing any files. Saving changes or taking a _snapshot_ of your work process is really important since you'll be able to track your changes over time rather than see one whole change. Another important thing is that by saving your change every so often you won't be able to lose your work unless you have autosave on. To be able to make a change you have to use `git status` to check if the file name is green before anything.

To be able to take a _snapshot_ of your code you have to set the code on stage so it can be _prepared_ to take a picture. You have to use the command `git add .` or specfic files by using `git add < file name >` to get them on stage so they can be able to save your file.

After when you add everything onto the stage by using `git add .` you have to be ready to take the picture which saving the change you have made into your file. By using the `command git commit -m "message"` you're saving the changes you by. The `-m "message"` means that you're are leaving a message so you can look back at the changes you have made by using `git log`.

---
## Workflow & Commands



Command | Explaination
---|---
`git init` | Initializes git in our directory which means making the folder into a parent function
`rm -rf < file name >` |  remove a file compelely
`git add .` | add a file onto the stage
`git commit -m "message"`| saves the changes you made and add a message
`git remote add origin URL`|Set the origin of the repo just in case if you used it to make other repos
`git push -u origin master`| This tells git to remember which remote repo & branch to push our changes to when we type git push in the future
`git push`|Send your code or _snapshot_ into a server
`git diff`|See the difference between your current code and you previous
`git log`|See your last commit
`git remote -v`|Tells you where git push will send your commits to (git status for your remote)
`git status`|command to see what files are staged for the commit








---
## Rolling Back Changes

#### Undo Edits

> To undo edits you have to first make some changes to a folder and do not add them to the stage nor commit. Do git status and your would see a chunk of words. Type the first command that was given to you and you'll be able to undo your edits

#### Undo add

> Go make changes to any file and do git add . to add them onto the stage. Then do git status and type the command onto of the green file name and you would undo the add and remove them from the stage

#### Undo commits

> What if you made a mistake and "accidentally" added a file onto the stage and commited the file. Don't worry check git status and do git reset --hard HEAD^ to undo a commit that was done by you. To undo multiple commits you can add a ~ and a number behind it to remove amount of commit you done.


