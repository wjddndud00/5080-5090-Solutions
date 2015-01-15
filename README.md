## Solutions to homework problems in Bain and Engelhardt's Introduction to Probability and Mathematical Statistics.

##### [Contents](#user-content-homework-solutions)

- [5080-5090 Solutions](#user-content-homework-solutions)
  - [Summary](#user-content-summary)
    - [Missing solutions](#user-content-missing-solutions)
  - [Adding and modifying files](#user-content-adding-and-modifying-files)
    - [Fork](#user-content-fork)
    - [Updating the repository](#user-content-updating-the-repository)
    - [Syncing the repository](#user-content-syncing-the-repository)
    - [Pull](#user-content-pull)
  - [LaTeX documents](#user-content-latex-documents)

### Summary

This repository contains solutions to homework problems assigned in Math 5080/5090 from the text, Bain and Engelhardt's Introduction to Probability and Mathematical Statistics.

To view solutions, open the PDF file.

To make contributions, you will need to add or modify LaTeX (*.tex) files. There is a master LaTeX file called Solutions.tex.
There is also a separate file for each homework problem. Solutions.tex calls each of the separate homework problem files to compile a single document will all the solutions. Thus if you want to fix or improve the solution to problem 5 from chapter 8, you will edit 05.08.tex and then compile Solutions.tex.

LaTeX files and Solutions.pdf will be tracked with Git.  Please do not commit other stuff, e.g. *.log files.

#### Missing solutions

Missing solutions (as of 12-7):
* Chapter 6: 17, 31
* Chapter 7: 5, 9, 10, 15, 17, 18, 19, 20, 22, 27, 28
* Chapter 8: 24, 26
* Chapter 9: 13, 19, 23, 24, 26, 31, 32, 33, 35, 36, 38, 39
* Chapter 10: 1, 5, 8, 10, 11, 12, 18, 20, 22, 25, 30, 31

### Adding and modifying files

[Git](http://en.wikipedia.org/wiki/Git_%28software%29) revision control software and a GitHub account are both required to contribute homework solutions. See [this video](http://youtu.be/ezxRcdJ8glM) for a step-by-step guide to setting up a GitHub account.

Git clients can be used from the command line and from GUI-based applications.

For the uninitiated, GitHub has easy to use GUI clients for [Windows](https://windows.github.com) and [Mac OS X](https://mac.github.com) that will make interacting with GitHub repositories much easier. There are other good GUI clients available, such as [SourceTree](http://www.sourcetreeapp.com).

Git repositories are organized into [branches](http://git-scm.com/book/en/v1/Git-Branching-What-a-Branch-Is), which keep track of the history and state of files that make up the repository. Generally, the first branch created in a repository is called **master**, and is generally considered to be the production branch. Read more about branches in this [tutorial](https://www.atlassian.com/git/tutorials/using-branches).

A [fork and pull collaboration model](https://help.github.com/articles/using-pull-requests) is used to add or modify the LaTeX files. 

#### Fork

To contribute your homework solution, start by copying or [forking](https://help.github.com/articles/fork-a-repo) this repository. Once you've copied the repository, download a local copy using the `git clone` command on the command line, or clone in a GUI app.

Add new LaTeX files for missing solutions, or modify an existing file to fix or improve a previously contributed solution as described above to your copy.

#### Updating the repository

Use the Git commands `add` and `commit` to [save your work](https://www.atlassian.com/git/tutorials/saving-changes/git-commit) either on the command line, or in a GUI client. Use the Git command `push`, again either on the command line or in a GUI, to update your remote repository on GitHub. [This tutorial](http://robert-reiz.com/2011/10/01/git-add-commit-push-pull/) is a good summary of all three commands. This [chapter in the Git book](http://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository) goes into more detail.

#### Syncing the repository

If working from the command line, or using a GUI client that does not support syncing from multiple remote repositories (the GitHub GUI clients do not), it will be necessary to sync your repository with this repository manually when this repository is updated. The commands are:

    git remote add upstream https://github.com/RonReeder/5080-5090-Solutions
    git fetch upstream
    git merge upstream/master

Here are the detailed GitHub instructions for [the `git remote` command](https://help.github.com/articles/configuring-a-remote-for-a-fork/) and [syncing the repositories](https://help.github.com/articles/syncing-a-fork/).

#### Pull

Create a [pull request](https://help.github.com/articles/creating-a-pull-request) to propose that the changes made to your repository be merged into this repository.

### LaTeX documents

The homework solution files are formatted using the [LaTex typesetting system](http://latex-project.org/intro.html) and used to generate the solutions PDF files.

Command line and GUI tools can be used to generate PDF files from LaTex.

For Windows, [MiKTeX](http://miktex.org) is an easy to use tool.
For Mac OS X, [TeXworks](http://www.tug.org/texworks) is also an easy to use tool.

A useful resource is the [LaTeX wiki book chapter on formatting math](http://en.wikibooks.org/wiki/LaTeX/Mathematics).
