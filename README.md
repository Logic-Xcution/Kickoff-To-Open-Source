[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)

![badge](http://img.shields.io/badge/first--timers--only-friendly-blue.svg?style=flat-square)

# KickOff To Open Source

Maintainer - [@MadhavBahlMD](https://github.com/MadhavBahlMD/)

First time open source seems very confusing.
So, here's a practise environment for your first contribution :D

**NOTE - CONTRIIBUTION TO THIS REPO IS NOT COUNTED AS A HACKTOBERFEST CONTRIBUTION. THIS IS JUST FOR PRACTICE.**

Also, you can see the presentation slides of `Kickoff To Opensource` here: [madhavbahl.tech/hacktoberfest2021/](http://madhavbahl.tech/hacktoberfest2021)

## Let's Start!

## STEP 1: Find The Project You Want To Contribute To

First step for starting open source is obviously, finding an open source project to contribute to!

Either you can go for contributing the project on some open source organisation like fossasia etc.

Or, you can find your projects/issues you want ot work on from these websites.

- [issuehub.io](http://issuehub.io/) - A website which helps you find projects/issues based on your required language or issue labels.

- [Code Triage](https://www.codetriage.com/) - Another useful tool for searching issues

- [Up For Grabs](https://up-for-grabs.net/#/) - List of projects with issues that can be resolved by beginners

- [First Timers Only](https://www.firsttimersonly.com/) - A list of issues that are labelled "first-timers-only".

- [Awesome First Timers PR](https://github.com/MunGell/awesome-for-beginners) - A list of awesome beginners-friendly projects.

By now, you must have found your required project/issue.

This is a first timers only repo which can be used to make your first open source contribution. We will write our username and description in the CONTRIBUTORS.md file and make a PR.

Congratulations! you just finished STEP 1

## STEP 2: Fork The Repository

Fork this repo by clicking on the fork button on the top of the page. This will create a copy of this repository in your account.

![image](https://user-images.githubusercontent.com/26179770/42131312-1bc9fe4c-7d1d-11e8-873a-be500dfd116e.png)

## STEP 3: Clone The Repository

Clone this repo to your machine. Go to your GitHub account, click on the clone button and then click the copy to clipboard icon.

Open a terminal and run the following git command:

```sh
git clone "Copied URL"
```

<img src="images/clone.gif" />

## STEP 4: Create A Branch

Go to the directory where you cloned the repo.

Create a new branch using `git checkout` command

```sh
git checkout -b <branch-name>
```

for keeping a standard, let's have the name of branch as username

for example:

```sh
git checkout -b MadhavBahlMD
```

<img src="images/checkout.gif" />

## STEP 5: Make Changes! Resolve Issue! Commit Those Changes! Push To GitHub!

Make the necessary changes, commit and push your code to GitHub.

Here, we are adding our username, name and bio in the CONTRIBUTORS.md

To make commit and push changes,

```sh
git add .

git commit -m "Add [username] as a contributor"

git push origin <branch name>
```

<img src="images/push.gif" />

## STEP 6: Open a Pull Request

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

Now submit the pull request!

Soon your changes will be reviewed and the PR will be merged if the changes are legit!

<img src="images/PR.gif" />

## Congrats

You just made your first PR.

Welcome to the world of open source

## Additional Details: Keeping your fork synced with original repository

First of all, switch to the master branch, master branch is the main working branch which is supposed to have most updated code!

```sh
git checkout master
```

Now, add original repo's url as a new remote, say `original`

```sh
git remote add original git@github.com:Logic-Xcution/Kickoff-To-Open-Source.git
```

This is a way of telling git that another version of this project exists in the specified url and we’re calling it `original`. Once the changes are merged, fetch the new version of original repository.

```sh
git fetch original
```

Now, you need to merge the new revision of my repository into your master branch.

```sh
git rebase original/master
```

Now you can push these changes to your GitHub repo:

```sh
git push origin master
```

Also, since your changes are merged and your repo is updated, the branch you created for your contribution is no longer required and you can delete it!

```sh
git branch -d <brach-name>
```

```sh
git push origin --delete <branch-name>
```

## All The Best!

Now you know how to contribute to open source, go ahead champ!
