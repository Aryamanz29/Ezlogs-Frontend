# Contributing Guidelines for Ezlogs-Frontend

| Index                                                         |
| ------------------------------------------------------------- |
| [Contributing to Ezlogs-Frontend](#contributing-to-ezlogs-frontend) |
| [We Develop with Github](#we-develop-with-github)           |
| [Report bugs using Github's issues](#report-bugs-using-githubs-issues)|
| [Basics of Git and GitHub](#basics-of-git-and-github)|
| [Fork a project](#fork-a-project)|
| [Clone the forked project](#clone-the-forked-project)           |
| [Add a remote (upstream) to original project repository](#add-a-remote-upstream-to-original-project-repository)           |
| [Synchronizing your fork](#synchronizing-your-fork)           |
| [Create a new branch for a feature or bugfix](#create-a-new-branch-for-a-feature-or-bugfix)           |
| [Push code and create a pull request](#push-code-and-create-a-pull-request)           |


## Contributing to Ezlogs-Frontend

We love your input! We want to make contributing to this project as easy and transparent as possible, whether it's:

- Reporting a bug
- Discussing the current state of the code
- Submitting a fix
- Proposing new features
- Becoming a maintainer

## We Develop with Github

We use github to host code, to track issues and feature requests, as well as accept pull requests.

## We Use [Github Flow](https://docs.github.com/en/get-started/quickstart/github-flow), So  that all the Code Changes Happen Through Pull Requests

Pull requests are the best way to propose changes to the codebase. We actively welcome your pull requests:

1. Fork the repo and create your branch from `master`.
2. If you've added code that should be tested, add tests.
3. If you've changed APIs, update the documentation.
4. Ensure the test suite passes.
5. Make sure your code lints.
6. Issue that pull request!

## Report bugs using Github's issues

We use GitHub issues to track public bugs. Report a bug / feature / doc changes by [opening a new issue](https://github.com/Aryamanz29/Ezlogs-Frontend/issues/new/choose); it's that easy!

Write issue with detail, background, and sample code.

**Great Issues** tend to have:

- A quick summary and/or background
- Steps to reproduce
  - Be specific!
  - Give sample code if you can.
- What you expected would happen
- What actually happens
- Notes (possibly including why you think this might be happening, or stuff you tried that didn't work)

- Use a Consistent Coding Style

## Basics of Git and GitHub

### Git & GitHub

Before we proceed, it's better to know the difference between Git and Github. Git is a version control system (VCS) that allows us to keep track of the history of our source code , whereas GitHub is a service that hosts Git projects. 

We assume you have created an account on Github and installed Git on your System.

Now enter your name and E-mail (used on Github) address in Git, by using following command.

`$ git config --global user.name "YOUR NAME"`

` $ git config --global user.email "YOUR EMAIL ADDRESS"`

This is an important step to mark your commits to your name and email.

<br />

### Fork a project

You can make a copy of the project to your account. This process is called forking a project to your Github account. On Upper right side of project page on Github, you can see -

<p align="center">  <img  src="https://i.imgur.com/P0n6f97.png">  </p>
Click on fork to create a copy of project to your account. This creates a separate copy for you to work on.

<br />

<br />

### Clone the forked project

You have forked the project you want to contribute to your github account. To get this project on your development machine we use clone command of git. You can also click on green `Code` Button and copy the URL from the dropdown.

`$ git clone https://github.com/<your-username>/Ezlogs-Frontend.git`

Now you have the project on your local machine.

<br />

### Add a remote (upstream) to original project repository

Remote means the remote location of project on Github. By cloning, we have a remote called origin which points to your forked repository. Now we will add a remote to the original repository from where we had forked.

`$ cd Ezlogs-Frontend`

`$ git remote add upstream https://github.com/Aryamanz29/Ezlogs-Frontend.git` 

You will see the benefits of adding remote later.

<br />

### Synchronizing your fork

Open Source projects have a number of contributors who can push code anytime. So it is necessary to make your forked copy equal with the original repository. The remote added above called Upstream helps in this.

`$ git checkout main`

This commands Navigates to Main Branch, if there are no changes made in the branch you're currently working with. 

`$ git fetch upstream`

This commands fetches all the branches and latest commits made in the upstream repository in the local system. The upstream is the remote pointing to the main repository on github.

`$ git merge upstream/main`

This commands merges all the commits from the upstream's main branch. 


`$ git push origin main` 

This command pushes the latest code to your forked repository on Github. The origin is the remote pointing to your forked repository on github.

<br />

### Create a new branch for a feature or bugfix

Usually, all repositories have a main branch that is regarded to be stable, and any new features should be developed on a separate branch before being merged into the main branch. As a result, we should establish a new branch for our feature or bugfix and go to work on the issue. 

`$ git checkout -b <feature-branch>`

This will create a new branch out of master branch. Now start working on the problem and commit your changes.

`$ git add -a`

This command adds all the files or you can add specific files by removing -a and adding the file name in place of `-a`.

`$ git commit -m "<commit message>"`

 This command gives a message to your changes so you can know in future what changes this commit makes. If you are solving an issue on original repository, you should add the issue number like #35 to your commit message. This will show the reference to commits in the issue.

<br />

### Push code and create a pull request

You now have a new branch containing the modifications you want in the project you forked. Now, push your new branch to your remote github fork. 

`$ git push origin <feature-branch>`

Now you are ready to help the project by opening a pull request means you now tell the project managers to add the feature or bug fix to original repository. You can open a pull request by clicking on green icon -

<p align="center">  <img  src="https://i.imgur.com/aGaqAD5.png">  </p>

Remember your upstream base branch should be main and source should be your feature branch. Click on create pull request and add a name to your pull request. You can also describe your feature.

#### Happy Coding 👩‍💻👩‍💻