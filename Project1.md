# Project Assignment 1
 
## Goals & Learning Objectives:
1.	Form a group
2.	Learn Git & GitHub
3.	Learn Markdown

## Assignment Specification:
This project assignment lays the groundwork for future project assignments. In this assignment you will form your group and learn to use industry standard technologies git and Markdown.

## 1. Form a group (20 points)

* Each group will be comprised of 4 people. We will help you form a group, just let me know. 
* Though not encouraged, there could be a team with 3 or 5 people in a team during the semester under certain conditions.
    * E.g. There is a student who drops the class. The team will become 3 people. 
    * E.g. There are two students in the same team and both drop the class. Then the remaining two students will be assigned to two other teams.
    * ...

* Deliverables: 
    Using the template provided, include:
    * Group Name
    * Name and pid of each group member

## 2. Learn Git & GitHub (50 points)
Git has become the de-facto standard for source version control in the IT industry. Your group will use a git repository to house your project. Submissions for grading will consist of a URL for a git repository and commit hash.

* Warm up
As a warm-up for this section, browse through https://git-scm.com/book/en/v2 and read the following sections:
    * 1: Getting Started 
    * 2: Git Basics
    * 5.1 Distributed Git - Distributed Workflows (your project will use the Centralized Workflow)
    * Or any other online resourcse for you to be familiar with Git. 

* Create Group repository
Each group member should create an account on https://github.com/. 
Choose a group member as Github manager who will host your group's work in GitHub. That group member (only) should:
    * Go to [Project_template](https://github.com/VTCourses/Project_template) 
    * Click `Use this template`
    * Project path should be `https://github.com/<your github account>`
    * Project name should be `cs4604-<groupname>`
    * Visibility Level should be *Private* 
    * Click on `Create repository from template`
    * Browse to `https://github.com/<your github account>/cs4604-<groupname>`
    * In the left hand menu select `Settings -> Manage access` 
    * Select the `Invite a collaborators` add:
        * pids of all group members & TAs (jeffchanAtVT, mrumi) & Instructor (yinlinchen)
        

At this point, each member of the group should be able to clone (or pull if already cloned) the project and see the working code. The normal workflow for a developer to push code to the central repository will be something like:

```
git clone git@github.com:<your github account>/cs4604-<groupname>.git
cd cs4604-<groupname>
git checkout -b newupdate master
<edit code>
git add <files/dirs to be committed>
git commit -m "some comment about commit"
git pull
git push origin newupdate
```

* Some tips:
    * [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
    * Occasionally you may have a merge conflict. Resolving the conflict will require communicating with your group members to make sure you are keeping the right code. See here for the mechanics of resolving the conflict: https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/
    * Commit early and often
    * If your local copy of the repository gets messed up, just delete it and re-clone. (Note that this will destroy any changes that have not been pushed to the central repository!)
    * Check [GitHub document](https://docs.github.com/en)!
    * Ask for help!!

## 3. Learn Markdown (20 points)

Markdown is a lightweight markup language with plain text formatting syntax. It is designed so that it can be converted to HTML and many other formats using a tool by the same name. Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor. See [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

Using Markdown, edit the README.md in your project's repository. Make sure it contains at least the following:
    * Team Name
    * Name and pid of all team members

Don't forget to commit and push your code!

## Submitting your work
One (and only one) team member should submit for the team. The submission should contain the ssh URL for your team's git repository and the commit hash you wish to submit for grading.

The commit hash can be obtained by one of the following methods:
* use the "git log" command at the command line
* browse to your project in `github.com/<your github account>/<projectname>` and click on the repository's Commits.  You will see a list of commits along with the hash. 

Sumbit below two items via Canvas.
1. Team GitHub URL: `https://github.com/<your github account>/cs4604-<groupname>`
2. GitHub commit hash URL. e.g. `https://github.com/<your github account>/cs4604-<groupname>/tree/5542903eb2e3a262a5ab32282997fde9fcb17c9e`