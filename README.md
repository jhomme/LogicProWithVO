# Workflow For Creating The Site

## Introduction

This is a totally accessible procedure for creating a website on GitHub using the Hugo static site generator and using Hugo to make GitHub pages. This procedure works on whatever operating system you use as long as you follow the installation instructions for each piece of software for your operating system.

## Prerequisites

- Go to <https://github.com> and sign up for an account.
- Go to<https://git-scm.com/book/en/v2>.
- Follow the first chapter there to install and set up git.
- Install Hugo using the instructions at <https://gohugo.io/installation/>.
## The Procedure

### Set Up Your Repository

- Go to GitHub and create a repository there.
- Copy the line that it shows as the repository URL to the clipboard by pressing the button.
- Go to your PC and get a command line.

## Set Up Your Local Repository

For this procedure, we will use SiteName to refer to the website you will create and UserName to refer to your user name on Github.

Below is a series of commands. You will input these into the command line on your computer. On the first line will be a command. On the next line will be what it does. After the second line for each command, is a double-space.

```
md websites
Creates a folder to hold your websites in case you want to make more than one.

cd websites
Switches into the websites directory

hugo new site website

 cd website

git add .

git commit -m "First commit of the site."

git push --set-upstream origin master

Since we have our public repository settings open in a new tab, go down to the github pages heading. Find the next heading that says, build and deployment.
Change the source to deploy from a branch.
Change the branch source to be, main, and make sure to select root for that second button next to the main.
Press save, and now you don’t have to touch these settings again! Now, when we publish your website, using whatever engine we want, it’s going to automatically
publish our website when we push our changes later.

In windows explorer, navigate to the hugo website directory we’re building. You should see a hugo.toml file that isn’t in a folder. Open this file in notepad.
Once hugo.toml is open in notepad, change the following, making sure to keep the tick marks around the words after the equal sign.
Replace the base URL, example dot com, with your public repository website URL like this, making sure to put your github username in the URL instead of
having it say, username.

https://LogicProWithVO.github.io/

Next, change the site title, keeping the tick marks around your title.
Save, then close this settings file.

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

CD $home/documents/website/username.github.io

git add .

git commit -m "Updated website"

git push
```