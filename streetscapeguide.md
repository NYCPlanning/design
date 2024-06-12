# Streetscape Installation Guide

This is a guide on the steps to install and run Streetscape, DCP’s digital design system on a [Storybook](https://storybook.js.org/) website. The current instructions are catered to MacOS and for those unfamiliar with using the command line.  

 

## Common Terminal Line Commands 

Here are a list of common commands that will be used throughout this process that will be useful to refer: 
* `cd` - used to change the working directory of the working drive or another lettered drive (aka the current folder you are in which is default should be user account)
    - `cd ..` - this command will go to the previous directory you were in
    - `cd pathname` - to go to a specific folder you will type cd and then the pathname of where you would like to go, i.e. if i want to go to my Documents, `cd Documents`
* `ls` - lists all the files and folders in the directory you currently are in
* `pwd` - prints the path you currently are in (aka the address of where you are now), this is useful if you do not know the pathname for one of the commands above

## Cloning a Git Repository
If this is your first time configure git in your terminal we will follow these steps: 
- Open your terminal and run the command `git config --global user.name "Your Name"`
 - Then run the command `git config --global user.email "you@example.com"`
This sets up your username and email associated to github.


If this isn't your first time, just to make sure we have the correct github account in terminal:
* Open your terminal and run the command `git config -list -show-origin`
    - this should output your github settings, make sure it has the correct user.email and user.name to the associated account you have on github

Now we should go to the directory you want to clone your repo to. To store in your documents folder run the command `cd Documents`

On your web browser, open to the [Storyboard Repo](https://github.com/NYCPlanning/ae-streetscape/tree/main). Now click the green code button on the website and copy the url for the HTTPS section.

- Go back to terminal and run the following command to clone our repo `git clone "the url link you copied"`

You've clone a repo! The next steps is to install npm to install our packages to run streetscape.

## Installing NPM

To install npm to download the packages needed to run streetscape we will need to use [nvm](https://github.com/nvm-sh/nvm). We will follow the same steps as Cloning a Git Repo except replace `cd Documents` with `cd ..`

Now follow the same steps as before. Once nvm is installed, we can install npm:
- run  `npm install -g npm`
- then `cd Documents/ae-streetscape`
- run `npm install` to install packages
- final step to run the env,`npm run dev`.


The streetscape website should pop up! To stop running it locally on your device you can hit the ^ and C key. 