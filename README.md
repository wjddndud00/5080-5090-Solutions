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

Missing solutions (as of 12-7-2014):
* Chapter 6: 17, 31
* Chapter 7: 5, 9, 10, 15, 17, 18, 19, 20, 22, 27, 28
* Chapter 8: 24, 26
* Chapter 9: 13, 19, 23, 24, 26, 31, 32, 33, 35, 36, 38, 39
* Chapter 10: 1, 5, 8, 10, 11, 12, 18, 20, 22, 25, 30, 31

#### Incorrect Solutions

Some of the incorrect solutions (as of 1-31-2015):
* 6.1b The correct density function is obtained but the work is sketchy.  W and w are used interchangably and the cdf needs to be defined as a piecewise function.  Currently there is no consideration of what the cdf would be for negative arguments. An extra d/dw appears and should be removed.
* 6.1c X and x are used interchangably.  Z and z are used interchangably.  The inequality in the solution should be strict.
* 6.1d Density function is not obtained and the work that is done is not done carefully.
* 6.2a The work is not carefully done.
* 6.2b z, w, and W are used interchangably.  Negative arguments to the cdf are not considered.  An extra d/dw and and extra =-1/w need to be removed.

### Adding and modifying files

[Git](http://en.wikipedia.org/wiki/Git_%28software%29) revision control software and a GitHub account are both required to contribute homework solutions. See [this video](http://youtu.be/ezxRcdJ8glM) for a step-by-step guide to setting up a GitHub account.

Git clients can be used from the command line and from GUI-based applications.

For the uninitiated, GitHub has easy to use GUI clients for [Windows](https://windows.github.com) and [Mac OS X](https://mac.github.com) that will make interacting with GitHub repositories much easier. There are other good GUI clients available, such as [SourceTree](http://www.sourcetreeapp.com). Git packages are widely available for Linux.

Git repositories are organized into [branches](http://git-scm.com/book/en/v1/Git-Branching-What-a-Branch-Is), which keep track of the history and state of files that make up the repository. Generally, the first branch created in a repository is called **master**, and is generally considered to be the production branch. Read more about branches in this [tutorial](https://www.atlassian.com/git/tutorials/using-branches).

A [fork and pull collaboration model](https://help.github.com/articles/using-pull-requests) is used to add or modify the LaTeX files. 

#### Fork

To contribute your homework solution, start by copying or [forking](https://help.github.com/articles/fork-a-repo) this repository. Once you've copied the repository, download a local copy using the `git clone` command on the command line, or clone in a GUI app.

Add new LaTeX files for missing solutions, or modify an existing file to fix or improve a previously contributed solution as described above to your copy.

#### Updating the repository

Use the Git commands `add` and `commit` to [save your work](https://www.atlassian.com/git/tutorials/saving-changes/git-commit) either on the command line, or in a GUI client. Use the Git command `push`, again either on the command line or in a GUI, to update your remote repository on GitHub. This [tutorial](http://robert-reiz.com/2011/10/01/git-add-commit-push-pull/) is a good summary of all three commands. This [chapter](http://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository) in the Git book goes into more detail.

#### Syncing the repository

If working from the command line, or using a GUI client that does not support syncing from multiple remote repositories (the GitHub GUI clients do not), it will be necessary to sync your repository with this repository manually when this repository is updated. The commands are:

    git remote add upstream https://github.com/RonReeder/5080-5090-Solutions
    git fetch upstream
    git merge upstream/master

Here are the detailed GitHub instructions for [the `git remote` command](https://help.github.com/articles/configuring-a-remote-for-a-fork/) and [syncing the repositories](https://help.github.com/articles/syncing-a-fork/).

#### Pull

Create a [pull request](https://help.github.com/articles/creating-a-pull-request) to propose that the changes made to your repository be merged into this repository.

### LaTeX documents

The homework solution files are formatted using the [LaTeX typesetting system](http://latex-project.org/intro.html) and used to generate the solution PDF file using LaTeX processing tools, either on the command line or in GUI applications. The [LaTeX wiki book](http://en.wikibooks.org/wiki/LaTeX/Basics) has a more detailed explanation of how LaTeX files are transformed into PDF files. This [tutorial](http://www.andy-roberts.net/writing/latex) is also a good introduction.

For Windows, [MiKTeX](http://miktex.org) is an easy to use GUI-based tool. For Mac OS X, [TeXworks](http://www.tug.org/texworks) is also a good GUI-based tool. LaTeX packages and utilties such as `pdflatex` are widely available for Linux. Here is a short `pdflatex`  [tutorial](http://www.thelinuxdaily.com/2011/08/how-to-build-a-tex-file-to-pdf-on-linux/).

Math symbols and formulas can be inline with text or displayed separately. Formatting is done through special enviroments containing the typesetting symbols and commands. This short [tutorial (PDF)](http://www.mecmath.net/latex-tutorial.pdf) demonstrates the use of frequently used math symbols and environments. This short [LaTeX course](http://www.math.uiuc.edu/~hildebr/tex/course) may also be helpful.

A very useful resource is the [LaTeX wiki book chapter on formatting math](http://en.wikibooks.org/wiki/LaTeX/Mathematics). See also this [comprehensive list](http://www.howtotex.com/general/12-great-resources-for-getting-started-with-latex) of LaTeX resources.

