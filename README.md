# GitHub Tutorial

_by Ryan Chen_

---
## Git vs. GitHub

_What is the Git and Github?_

Git and GitHub are separate from one another even though they are used together. They may have the word "Git" but they function completely different from one another. Git acts more like a tool that keeps track of the changes you make while you're programming where you're able to look back what you've done. On the other hand, Github is used is a server that stores all your information digitally so you can access it anywhere rather than locally where it only available in your laptop/device.

**Git** | **GitHub**
---|---
Access Locally | Access Globally
Doesn't requires wifi | Requires wifi
It's on your computer | Collaboration with other

_What is a repo? Local vs Global?_

Repo is a short acronym for a repository, but you would wonder what is a repo and what does it do. A repository is a place where information can be stored and can be accessed later on. In this case, a repo is stored in GitHub where your project can be accessed anywhere with connection with wifi. This leads up to the questions what the difference between a local repo and a global repo. A local repo can only be accessible within the device that you store the information in and in order to share it you either have to store it within a server, but with a global repo, you can store it and access it in a different computer that isn't you own which is convenient.


---
## Initial Setup

Before we start getting into git you'll have to make a Github account and set up your ide, which is an additional step you need to do. If you haven't already go GitHub and create an account or click [here](http://github.com) then you'll need to set up your ide which we're going to do after.

1. You need to enter your information
    * Register an account by making a username, password, and entering your email address
    * Choose a wise username and password so you can remember it later one when you're logging back on

2. Choose the beginner plan **(It's free)**

3. Complete your setup
    * Answer the question to your own personal preferences and click the _complete stepup_ button whenever you're done. This is really an optional step so you can do it if you want or not

4. Verify your email
    * Go log on your email and verify your Github account to make your that you're the person who made the account and not anyone 


After when you finish making your Github account you need to set up your ide which stands for an **integrated development environment** which is the place that you'll be writing your code in and your work. An ide is a sandbox that you have at your disposal that you can mess around without making any mistake whatever you want. Rather than using your terminal on your computer, an ide is much safer since making mistake won't harm your computer then the terminal where it can do permanent damage on your computer. There other ides that you can run your code in but we're are working with this one since it's free; however every ide is different since it all works differently were there benefits and drawbacks. 

Go to [IDECS50](ide.cs50.io) and log in with your GitHub account and follow the steps [here](https://github.com/hstatsep/ide50) to set up your IDECS50

> ### Whats is SSH?
> SSH stands for Secure SHell which goes through a protocal to help someone safety access the net.

---
## Repository Setup

Before anything, you need to initialize your git, create a directory that your file will contain at by using `mkdir < File Name >`. A directory is a library that stores your information or project within such as files, documents, images, and videos. After you initialize your git you would need to `cd < file name >` to make any changes within the directory. Then you would need to do `git init` to initialize the git which makes the file into the parent function of every other. This also means that you can store anything within where it's considered as the `(master)` in your code.

As you start making changes to your files start checking what you have done by using `git status` to see the changes that you're making before you're committing any files. Saving changes or taking a _snapshot_ of your work process is really important since you'll be able to track your changes over time rather than see one whole change. Another important thing is that by saving your change every so often you won't be able to lose your work unless you have autosave on. To be able to make a change you have to use `git status` to check if the file name is green before anything.

To be able to take a _snapshot_ of your code you have to set the code on stage so it can be _prepared_ to take a picture. You have to use the command `git add .` or specific files by using `git add < file name >` to get them on stage so they can be able to save your file.

After when you add everything onto the stage by using `git add .` you have to be ready to take the picture which saving the change you have made into your file. By using the `command git commit -m "message"` you're saving the changes you by. The `-m "message"` means that you're are leaving a message so you can look back at the changes you have made by using  `git log`.

---
## Workflow & Commands

After you set up your Github and ide you can already start writing your code by using the thing that was said in the repo set up, but we'll be going over it again to make sure that you're getting the hang of it. When you're working no matter which step you're in always do `git status` to check what was edit and change so you'll be able to track your changes over time. 

Start by making a directory that you'll be working on by using the command `mkdir < file name >` and go into the folder by using `cd < file name >`. Now follow closely make your folder into a parent function by using `git init` so you can start adding stuff into it and now pay attention do `touch < file name >` to make a file that you'll be making edits in; for example, a google docs that you can write your stuff in. Follow by that do `c9 < file name> ` to get into it so you can start by making some changes.

When you finish making your changes you have to add them on to the stage before taking a _snapshot_ do `git add .` to add your change onto the stage so it can be prepared. After you add them onto the stage do `git commit -m "< message >"` to commit your change and don't forget to add a message so you can be able to track your change later. Always check `git status`!

Now, what do you do after you make your commits? You wonder can you show off your awesome work to the public? Yes, you can. Go log on Github if you haven't and go to the top left corner of the page you'll see a green button that says `new`. Click that to make a new repo so you can store in within a server rather than locally within your computer which can get lost. After you click the green button name your repo the same name as your parent function and add a description if you want. Check the box below if you want to make the repo online if you want but right now we did not so don't check it off. Copy the first link it should look like this `git remote add origin git@github.com:< your username >/kjwd.git` and after copy the second link `git push -u origin master` to push it into Github. When you finish you're all done and don't forget to always to `git status` to check your progress, also to present your great work always also do `git push` to push it to Github.

If you ever make a mistake you would start panicking but don't worry `rm -rf < file name >` is here to save you. You can use that to delete a file if you can a mistake and want to redo everything; however, it's a double edge sword because you can accidentally delete everything so be careful whenever you are using it. Since you read all the through here I'll give you an extra thing you can use that can benefit you. If you ever want to change the name of your directory use `mv < current name > < new name >`.


In the bottom is some additional command that you might need when you are programming but I won't go in-depth into them so take a look or quick glance at them.


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

Let me give you a scenario that happens if you stage someone you don't want to stage and want to kick them off or you already took a picture that you weren't meant to take you do have a chance to redo your mistake! Even though you can use `git log` and `git revert` to go back to your last commit but it can't work in every scenario since what if you only want to make a small change back and don't want to make a huge jump back to the beginning. You can use `git checkout -- < file name >` to undo a stage that you have added neat right. Do `git status` once more to check if your file change from green to red so you can know that you had made changes. To double-check used `git diff` to see your current and compare to your previous to see what had changed.

What if you already check them out and took their picture and you regret that you have done it. You want to remove the picture of the camera. Used the command `git reset --hard HEAD^` to undo a commit you have already done. To undo multiple commits add the number after heading for example HEAD ~ 1, etc. Just make sure that you're looking back at your previous commit just in case if you don't make a mistake.

You can just always do `git log` and then `git revert < numbers >` if you didn't make much change. In below are brief explanations if you don't understand what I've said above.

#### Undo Edits

> To undo edits you have to first make some changes to a folder and do not add them to the stage nor commit. Do git status and your would see a chunk of words. Type the first command that was given to you and you'll be able to undo your edits

#### Undo add

> Go make changes to any file and do git add . to add them onto the stage. Then do git status and type the command onto of the green file name and you would undo the add and remove them from the stage

#### Undo commits

> What if you made a mistake and "accidentally" added a file onto the stage and commited the file. Don't worry check git status and do git reset --hard HEAD^ to undo a commit that was done by you. To undo multiple commits you can add a ~ and a number behind it to remove amount of commit you done.


