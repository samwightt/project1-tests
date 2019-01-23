# Project 1 Tests
Test cases for UA CS101 Project 1.

# Important Note about UA's Code of Academic Conduct
Under no circumstances should **any of your project code be attached to any of the test cases you submit here**. Code of any kind **should not be posted in any of the issues, wiki, projects, or other parts of this repo**. This is **against UA's Code of Academic Conduct**. All Academic Conduct violations will be reported to the appropriate authorities.

Again, *just one last time so that we're clear*: **you should not include any code in any test cases, commits, pull requests, issues, wiki edits, issue comments, commit comments, etc.** This repo is **solely** for test cases and output results; you are not allowed to discuss or share anything about **how you acheived those results**, only about the results themselves. Any content infringing this **will be removed, and you will be reported to our professor and the Office of Academic Affairs**.

**I do not condone breaking the Code of Academic Conduct. The purpose of this repo is to help students verify their results, and not to condone, promote, or allow cheating or plagiarism. I am not responsible for any negative repercussions you may face if you break this policy.**

## What is this? 

This is a Git repository for UA CS101 students to collaborate on test cases for Project 1. You can download and test any of the test cases here, and check the issues tab to find the expected results. If your results differ, you can post in the specific issue as well, and other students can help you fix the problem if possible. 

You can also submit your own test cases along with expected results so that other people can verify it with their implementation. See below for how to do this.

## Cool! How do I use this?

First, you'll need to install Git on your computer. Git is a version management system that allows you to keep a timeline of all of your file edits. Think of it like undo/redo, but for your codebase. If you accidentally save a change that you didn't mean to, you're able to undo it by reverting to a previous version. [Here's how to install Git for your platform.](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

Next, you'll need to initialize a Git repository in your code base. To initialize a Git repository in your existing code base, run the following commands:

    cd ~/path/to/your/project/folder
    git init

After this, you'll want to *commit* all of your existing changes. [See this link for more information about Git and how commits work.](https://medium.freecodecamp.org/what-is-git-and-how-to-use-it-c341b049ae61). To do this, run the following commands:

    git add .
    git commit -m "My first commit!"
    
Congratulations! You just made your first commit. 

Finally, you'll want to add this git repository as a *submodule* to your current repository. All a submodule does is download a git repository into a subdirectory of your code. Run the following commands to add this repository as a submodule:

    git submodule add https://github.com/samwightt/project1-tests tests

This command will download this git repository (`samwightt/project1-tests`) into a folder called tests in your project folder. Congratulations, you can now run the tests!

## Great! How do I run the tests?

You'll have to run the tests indivdually and verify the results yourself. If you used the above commands, all the tests should be in a `tests` subdirectory underneath your project folder. Use a command like this to run them:

    ./project1 tests/test1.txt

## How do I verify the results?

To verify the results of a test, you'll want to check out the **Issues** page on the Github repository. There you'll want to find the issue corresponding to the specific test case. Each issue will contain how to run the test case, the expected output, and a set of inputs with expected outputs. You can verify these against your own code and see if there are any problems.

## Some new test cases were added. How do I download them?

Just pull the latest changes from the remote using `submodule update`:

    git submodule update --remote

## How do I contribute my own test cases?

To contribute your own test cases, you'll need to submit a pull request on Github. [See this link to learn how to do so.](http://oss-watch.ac.uk/resources/pullrequest) You'll need a Github account, as well as a copy of your forked version of the repository (click 'Fork' at the top). Download the forked directory to your computer like so (make sure you're not in your project directory!):

    git clone https://github.com/yourusernamehere/project1-tests
    cd project1-tests

Now, add any of your test cases to the directory. Make sure to rename them using the numbering scheme (test#.txt, where # is the next largest number). Last, commit the files and push:

    git add .
    git commit -m "Added test case #."
    git push origin master

Finally, submit a pull request to this repostitory, along with some inputs and expected outputs. Once you do that, your submission will be reviewed, an issue will be created for your test case, and the commit will be merged into the repository!

## Help! I'm having trouble with something!

If you're having trouble with anything, don't hesitate to reach out to me. You can reach me in the CS 101 GroupMe, or you can just make a new issue here. Before you reach out, make sure to look through the issues here to see if the question hasn't been asked already (just to lower question volume as much as possible). After that, ask away!

# Important

**Please make sure you read the note at the top of this README.** It is **extremely** important that you know that cheating will **not** be tolerated.
