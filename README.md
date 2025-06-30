# ENGS 96 Mathematical Foundation for Machine Learning - Course Assignments

## Student data

Name: 'YOUR NAME HERE'
Email: 'YOUR EMAIL HERE'

Carefully follow the instructions below to setup your assignment repository.

## Assignments Overview

* [Assignment 1](assignment1) (Due date: July 9)
* [Assignment 2](assignment2) (Due date: July 28)
* [Assignment 3](assignment3) (Due date: August 11)
* [Assignment 4](assignment4) (Due date: August 25)

## General Rules and Instructions

### Plagiarism Note and Late Policy
Copying code (either from other students or from external sources) is strictly prohibited! Late submissions will generally not be accepted. In case of serious illness or emergency, please notify TA team under `matthew.t.khoo.25@dartmouth.edu`

### Publishing Code on Personal Git Repositories
We explicitly ask you to not create any public repositories containing copies of these assignments or solutions to them. In any case do not include any terms that are identifiably related to this course and make the repository easily searchable.

### External Packages
Please use external libraries with caution.
Most packages can be used unless they directly solve or significantly help with the task.
If in doubt, please ask the TA team about package usage or create a thread under the discussion forum.

### Installing Git
Before we can begin, you must have Git running, a distributed revision control system which you need to hand in your assignments as well as keeping track of your code changes.
We refer you to the online [Pro Git book](https://git-scm.com/book/en/v2) for more information.
There you will also find [instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git]) on how to install it.
On Windows we suggest using [git for windows](https://git-for-windows.github.io/).

### Cloning the Assignment Repository
Before you are able to clone your private assignment repository, you need to have an active [Github](https://github.com/) account.
Then you can **create your own private online repository** by following this link: [here](https://classroom.github.com/a/jh3feDB2)

In the next step you need to clone it to your local hard drive
```
git clone --recursive https://github.com/ENGS-96-summer25/engs96-'Your_Git_Username'.git 
```
'Your_Git_Username' needs to be replaced accordingly. This can take a moment.


Next, cd into the newly created folder, and add the base assignment repository as a remote:
```
cd engs96-'Your_Git_Username'
git remote add base https://github.com/ENGS-96-summer25/engs96-template.git
git pull base main --allow-unrelated-histories
```
Now you should have your local clone of the assignment repository ready. Have a look at the new repository folder and open the 'README.md'. It contains the text you are just reading. Please fill in your name and student number at the top of this file and save. Then you need to stage and commit this changed file:
```
git add README.md
git commit -m "Adjust README.md"
git push
```
You should now be able to see your name online on your private repository: https://github.com/ENGS-96-summer25/engs96-'Your_Git_Username'

### Workflow
In general, you should use Git to commit your edits as often as possible. This will help you with backtracking bugs and also serve as a backup mechanism.
For more information we refer you to the [Pro Git book](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository).

Every new assignment needs to be pulled from the base repository:
```
git pull base main
```
or,
```
git pull base main --allow-unrelated-histories
```

### Solution Submission
In every assignment directory you will find a 'README.md' file in which we will specify the required screenshots and console outputs. You should briefly summarize and report your results and observations, or discuss possible problems.
For a quick introduction of the Markdown syntax see: https://guides.github.com/features/mastering-markdown/

To submit your solution of the assignment please add the following commit message: "Solution assignment X". E.g:
```
git commit -m "Solution assignment X"
git push
```
You can keep updating your code before the deadline. After the deadline, please don't change the code before we send you the scores.

**The solutions must be submitted before the deadlines mentioned in the assignment sheet and on the course website. Late submissions will not be accepted.**
Collapse
