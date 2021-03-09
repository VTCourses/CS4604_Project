# Project Assignment 3

The goal of this final project is to interface your database with a programming language and to make it web-accessible. This is the stage where you embed your database into a complete application. You can choose the programming language you would like to build your project, or PHP - a general-purpose scripting language especially suited to web development. You can also use your own database or a PostgreSQL database that has been installed on cs4604.cs.vt.edu. We can also provide AWS resources for you to use, contact your Project TAs with detailed requests.

Important: If you choose to use your own programming language and database. Your team takes full responsibility for ensuring that your machine supports all the desired functionalities. We will NOT be able to accommodate any last-minute requests for extensions because something is not working. We provide this option for your convenience so that you can take advantage of any already existing setup for your project. Do not attempt this unless you are absolutely positively sure of what you are doing. We do not have the resources or the manpower to provide technical support and help in debugging. At the end of the day, we will grade it just like every other project.

## Goals & Learning Objectives:
* Learn the advanced database design, database normalization, and perfect the relational schema.
* Learn about and use a database management system e.g., PostgreSQL, MySQL, etc.
* Practice database querying by posing advanced queries using SQL directly and also indirectly using a program.
* Write a database Web application with creative and useful functionalities.

## Deliverables:
1. Every group should turn in a final project package, including application code, dataset, SQL files, a final project report, and presentation slides, etc.
2. Every group should give an 8 minutes presentation with a demonstration of project Website in class.
3. Self and Peer evaluation form. (We will release this form after project presentations. [Preview](STUDENT_PEER_EVALUATION_SHEET.pdf))

    Note: While grading your solutions, we will pay attention to the quality of your codes, SQL files, documentations e.g., whether they are correct and functional, software and database complexity, and the running time (performance).


## Q1. E/R diagrams and relational schemas refinement [20 points]

In this question, refine your E/R diagram and relational schemas using functional dependencies and normalization. Apply what you learn from the classes (Week 9: Functional Dependencies, BCNF, 3NF, and Normalization) and textbook and finalize your project's E/R diagrams and relational schemas. 

1. Make sure your E/R diagram accurately models the requirements of your project:
    * Define multiplicity and participation constraints for all relationships.
    * Setup identifying relationships for any weak entities.
    * Identify any requirements that it is not possible to model.

2. Make sure you convert your E/R diagram to a relational model. Provide both the diagram and the SQL for your relational model. 

    * Define data types correctly for each column
    * Set null/optional constraints for each column
    * Correctly define primary key and unique constraints (multiple unique constraints should be annotated with a label)
    * Correctly define foreign key constraints
    * Identify any requirements that it is not possible to model
    * Normalize your relational schema to 3NF or BCNF. Provide a proof showing what form your schema is in.
        1. List all completely non-trivial Functional Dependencies (FDs) that apply to that relation. Only list FDs that have one attribute on the right hand side. It is enough to list only the FDs in a minimal basis.
        2. For each FDs from (a.), write down if it is in BCNF. Explain each answer. If any of relations are not in BCNF, decompose and normalize them to BCNF.
        3. List any resulting relations from (b.) is in 3NF?
    
Put everything you have for this question into your final project report. E.g. E/R diagram and the details about any normalization and relational schema.

## Q2. Database and dataset [10 points]

Create SQL scripts to populate your database with the project dataset. Put SQL scripts in the project `sql/` folder and details each script in the project report. Put dataset or link to the dataset in the project `dataset/` folder and details describe the dataset.

1. A detailed step-by-step overview of database setup in the database section. 
    * SQL scripts to create tables
    * SQL scripts to import dataset

2. A dataset description 
    * Describe the dataset you use in your project. [Example](https://www.imdb.com/interfaces/).

Important: import only the data you actually use in the project. If the original dataset contains 10 tables and your application use only 5 tables, your SQL scripts and dataset description should only contain these 5 tables. Do not import and provide a dataset of all 10 tables into your database and report. 

## Q3. Develop a Web-based, Database-backed application [50 points]

Write a Web-based, database-backed application that meets the specification. Additionally, your application should allow a user to create, update and delete any entities in your relational model.

Assessment criteria: Is all functionality present? Does everything work correctly and do all the buttons and links that we click indeed do what they are expected to do? We will see if you are really accessing the database dynamically and are not just "looking up" the data from some ready made source. We will ensure this by typing ad-hoc queries. You will also need to make sure that all query results have column names neatly presented and that data is clearly tabulated. Your application should not have SQL injection vulnerabilities.

In your project report, clearly list exactly what you have implemented and how we can test it. Note that you must implement some extra functionality to have a chance of getting up to 50 points. Here are some suggestions for this step:
1. Implement more complicated DB functionality: inserts, updates, deletes, etc., or some more complex queries.
2. Create a more visual or sophisticated interface for your web application, not just the vanilla style template shown above. If there is a more "natural" way for your application, maybe you will write some nice interface for it.
3. Address other aspects of your application, such as transactions.
4. Use your creativity and implement some interesting functionalities!

Provide an application installation guide in your project report. 

## Q4 A project report and presentation [20 points]

Prepare a project report and presentation slides

1. A project report:

    Where you summarize all steps of your project in a single document. Include snapshots of your web interface. Making sure you include the E/R diagram, the details about any normalization, your relational schema and, the queries you created (above) in the previous steps of the project. Include the role of each team member in the project. Clearly identify the scope of everybody's contribution. Mention your project web-page on the first page of your report. Include your answer to the next question too.

    Your project report at least should contain these sections:

    1. Overview
    2. Objectives and accomplishments
    3. E/R diagram
    4. Relational schema
    5. Database and dataset
    6. Application
    7. Conclusion
    8. Appendices

2. A project presentation

    A presentation slides for your project presentation 

## Project GitHub Repository

Your project GitHub repository should, at a minimum, have the following directory structures and files:

* README.md - a file containing your project documentation. It must at least include all sections described in the [demo](https://github.com/yinlinchen/SuperHeros) project.
* code/ - a directory containing all of your source code.
* diagrams/ - a directory containing all model diagrams.
* sql/install.sql - a file containing the SQL necessary to create the database schema.
* sql/load.sql - a file containing the SQL necessary to load your schema with project data.
* dataset/ - a project dataset in a `zip` format file. If the file is larger than 100MB, please upload it to Google drive and put the file sharable link in the Readme.md.
* slides/finalreport.pptx - your final presentation file.
* docs/projectreport.pdf - a project report where you summarize all steps (with screenshots) of your project in a single document.

Note: See the demo project for a potential starting point: https://github.com/yinlinchen/SuperHeros

## The tangible steps you will take for project assignment 3 are:
* Read the project description again.
* Understand and explore the datasets you choose.
* Review and update personas for your application.
* Revise Entity-Relationship (ER) diagrams.
* Perfect the relational schema using FDs and normalization.
* Write SQL scripts to create the database and load the project dataset.
* Implement a functioning Website to present some complex relationships and useful functionalities.
* Prepare a project report and presentation slides.
* Assemble all your works and put them into your team project GitHub repository.
* Present an 8 minutes presentation about your project.

## Tips
* Generate random data for testing: e.g. https://mockaroo.com/  
* Try to construct data that could check for the following potential errors:
    * Incorrect output schema
    * Output may be missing rows from the correct answer (false negatives)
    * Output may contain incorrect rows (false positives)
    * Output may have the wrong number of duplicates.
    * Output may not be ordered properly.
* Prevent long running queries, revise relational schemas, create `view`, etc. 

## Submitting your work
One (and only one) team member should submit for the team. The submission should contain the ssh URL for your team's git repository and the commit hash you wish to submit for grading.

Create a release for project 3, see [How to create a GitHub release for a repository](github.md).

Submit GitHub release URL to `Project 3` in the Canvas.
1. GitHub release URL. e.g. `https://github.com/<your github account>/cs4604-<groupname>/tree/<version-number>`.  

## Bonus points

1. You will grade other teams according to their presentations. E.g., If your team's project is `FilmFanatic`, then you will grade `TooManyGames` and `TravelLover` teams' presentations.

    Three teams with the highest score will receive 10 bonus points for project assignment 3.

2. If the extra functionality is exceptional, you can get up to 20 points of extra credit, depending on how complex your application is.

## Project contact
Monjura Afrin Rumi (mrumi@vt.edu): 
* FilmFanatic
* PHP on Windows

Hongjie Chen (Jeffchan@vt.edu): 
* TooManyGames and TravelLover
* PHP on Mac / Linux

## Reference
* [SQL Style Guide](https://www.sqlstyle.guide/#white-space)
* [PHP Tutorial](https://github.com/VTCourses/PHP_tutorial)