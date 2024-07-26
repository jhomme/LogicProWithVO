# Workflow For Creating The Site

## Introduction

This is a totally accessible procedure for creating a website on GitHub using the Hugo static site generator and using Hugo to make GitHub pages. This procedure works on whatever operating system you use as long as you follow the installation instructions for each piece of software for your operating system.

## Prerequisites

- Go to <https://github.com> and sign up for an account.
- Go to<https://git-scm.com/book/en/v2> and bookmark that page.
- Follow the first chapter there to install and set up git.
- Install Hugo Extended using the instructions at <https://gohugo.io/installation/>.
- Go to <https://markdownguide.org> and get fmiliar with Markdown.

## The Procedure

### Set Up Your Repository On Github

- Go to GitHub and create a repository there.
- Copy the line that it shows as the repository URL to the clipboard by pressing the button.
- Go to your PC and get a command line.

## Set Up Your Local Repository and Website

For this procedure, we will use SiteName to refer to the website you will create and UserName to refer to your user name on Github.

Below is a series of commands. You will input these into the command line on your computer. On the first line will be a command. On the next line will be what it does. After the second line for each command, is a double-space.

```
md websites
Creates a folder to hold your websites in case you want to make more than one.

cd websites
Switches into the websites directory
```

- Type `git clone`, press **SPACE**, then paste from the clipboard and press **ENTER**.
- This sets up the repository you made from Github on your local computer.
- Type `cd ..`
- This backs you out one directory.

hugo new site website
Creates the site in the directory you made.

 cd website
Go into the website you made.

git checkout -b gh-pages

git add .

git commit -m "First commit of the site."

git push --set-upstream origin master

Site name below:

git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git

hugo

git add .

git commit -m "Publishing after adding the theme"

git push --set-upstream origin master

CD $home/documents/website/username.github.io

git add .

git commit -am "Updated website"

git push

hugo

git add .

git commit -m "Changed website"

git push

git add .

git commit -m "Updated website"

git push
```
echo "# LogicProWithVO" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/jhomme/LogicProWithVO.git
git push -u origin main
```
