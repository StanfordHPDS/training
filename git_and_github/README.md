# Git and GitHub

git is a tool for version controlling projects, and GitHub is a git-hosting service that allows for easy collaboration on git projects. 

This training will focus on two main mental models: the basics of how git works, focused on the command line interface, and the basics of collaborating with others on GitHub.

## Pre-work

There is a bit of work to make sure you've done for this training. In short, you want to make sure you have git installed and connected to GitHub.

We'll use [Happy git with R and RStudio](https://happygitwithr.com) as a reference, as it includes guidelines for how to set things up both using the terminal and using R/RStudio.

### Install and set up git

Even if you've never used git before, there's a chance it's already installed. Walk through the chapter on [Installing Git](https://happygitwithr.com/install-git) to check and install it if not.

Then, make sure git [knows who you are](https://happygitwithr.com/hello-git).

I also recommend taking this time to [change the name of your default branch](https://happygitwithr.com/hello-git#configure-the-default-name-for-an-initial-branch) to `main` by running this command in the terminal:

```bash
git config --global init.defaultBranch main
```

### Connect to GitHub

You'll also need to authenticate with GitHub if you haven't already. 

If you don't already have one, create an account on GitHub.

For git to interact with repositories hosted on GitHub, you'll need to authenticate at some point. A good way to do this is with a [Personal Access Token](https://happygitwithr.com/https-pat). 

If you're an R user, follow the set up on Happy Git. This will allow you to set up your credentials ahead of time.

If you're not an R user, you might need to [store your PAT somewhere secure](https://happygitwithr.com/https-pat#store-pat) for the next time git asks you to authenticate. 

Alternatively, you can authenticate using the [GitHub CLI](https://cli.github.com/) using `gh auth login`.

## Bonus setup: Git Clients

We'll use the command line interface for this particular training, but there are many git UI interfaces that are very helpful. RStudio and VS Code both have simple interfaces for creating repositories, making commits, and other straightforward features.

There are also a [number of more sophisticated apps](https://happygitwithr.com/git-client). [GitKraken](https://www.gitkraken.com/) is particularly nice, although many people prefer the [GitHub desktop app](https://desktop.github.com/).
