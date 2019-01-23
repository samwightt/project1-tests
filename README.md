# Project 1 Tests
Test cases for UA CS101 Project 1.

## What is this? 

This is a Git repository for UA CS101 students to collaborate on test cases for Project 1. You can download and test any of the test cases here, and check the issues tab to find the expected results. If your results differ, you can post in the specific issue as well, and other students can help you fix the problem if possible. 

You can also submit your own test cases along with expected results so that other people can verify it with their implementation. See below for how to do this.

The best part 

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
