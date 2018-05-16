Intro to Git[Hub]
========================================================
author: Josiah Parry 
date: 
autosize: true

What is Git?
========================================================

I will let the "Queen of Git 

 _"Git is a version control system. Its original purpose was to help groups of developers work collaboratively on big software projects. Git manages the evolution of a set of files – called a repository – in a sane, highly structured way. If you have no idea what I’m talking about, think of it as the “Track Changes” features from Microsoft Word on steroids."_ - [Jenny Bryan](http://happygitwithr.com/big-picture.html)

========================================================
width: 1920
height: 1080

![](images/vc-xkcd.jpg)


Get set up with GitHub
========================================================

Before we begin learning git, it will be helpful to have a place to work on our projects. We will all use a GitHub account.

Please go to GitHub (https://github.com/signup) and create an account. I recommend you use a personal email address that way you can still have access in the future.

**Remeber your username and password**, this will be necessary for connecting to git.

Installing
========================================================

Since we're all on Mac's it will be easy to install. Simply try running a git command, and if you have git, it will work. Otherwise, it will prompt you to install it.

1. Open the terminal. 
  - Press `command + space bar`. This will pull up spotlight search.
  - Type in `"terminal"`, press enter when the application has appeared.
2. Once inside terminal, type `git --version`. This will either tell you which version of git you have installed, or prompt you to install `xcode`.
  - If prompted, begin downloading.
3. If / once you have completed downloading, run `git --version` to double check that it is installed.


Configuring your Git
========================================================

* There is one more step necessary before you can make changes and push them to GitHub. 
* You need to connect your account to your machine. Do this by running the line below.
* Ensure that you've used the same username and email as you did when you created your GH account.


```r
git config --global user.name 'Your Name'
git config --global user.email 'personal@email.com'
git config --global --list
```

You're still confused, I get it. Me too.
========================================================









