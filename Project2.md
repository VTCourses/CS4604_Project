# Project Assignment 2
There are three projects: [FilmFanatic](projects/Project1.md), [TooManyGames](projects/Project2.md), [TravelLover](projects/Project3.md) for your team to choose. Please read each project's description carefully and make your choice. We will release a project sign-up form in Canvas on 4:40pm 02/11/2021. Each project has at most 6 teams to work in this semester. Each project team will have its own instance of the project data and will build a separate and unique interface to its instance.

## Goals & Learning Objectives:
Learn the essentials of database design
1. Create application specifications
2. Create Entity-Relationship diagrams
3. Convert ER to Relational model

## Assignment Specification:
* Please type your answers. Illegible handwriting may get no points, at the discretion of the grader. Drawings and diagrams should be created using Google Draw, LucidChart, [ERDPlus](https://erdplus.com/) or other appropriate diagramming tool.
* There could be more than one correct answer. We shall accept them all.
* Whenever you are making an assumption, please state it clearly.
* The most important thing is others can read and understand your document.
* Prepare the presentation, other students will grade your presentation.

## Q1: Application specifications (40 points)
According to the project description and dataset, write your application's personas and specifications 

* Q1.1 (8 points) Your application's personas. How the user use your application? What information will your user get from your application? 

    (Note: Write a description of the overall context or scenarios about your application. For example, if the choice is to work on a books database, you may describe your application as "the books available at a library" or "the books sold by a bookstore.".)

* Q1.2 (8 points) What are the application specifications i.e., what functionality will your completed system provide? 

    (Note: To give an analogy, suppose you were designing a web browser. Your answer might say that the browser will support visiting URLs, maintain a history of visited web pages, allow users to tag bookmarks, etc. Your answer will not need to go into the details of the positions of various menu items.)

* Q1.3 (8 points) What aspects of the application will your system model?

    (Note: For example, in the books domain, you can write something like "We will model books, authors, publishers, and printers" You must examine the dataset in order to get a sense of the information you need to model.)

* Q1.4 (8 points) Write some of the other "value-added" facilities your system could support? You can draw inspiration from the `Internet`, if you want. 

    (Note: For example, if this was a movie info system like IMDB, such a facility could be a "recommender system" that makes movie recommendations for users based on buying trends. In other words, the recommender system is a facility that will be enabled by the presence of a database system.)

* Q1.5 (8 points) What is the role of each project member in the project? 

    (Note: You don't have to "commit" to anything now. We want to see if any of the group members brings special talents/experiences to bear upon the project. For example, if one of you has worked in a digital store project, (s)he may help identify design choices from this point of view. If one of you has experience in web-based software development, then that would be a good thing to mention.)

## Q2: Designing the database (30 points)
According to the project description and personas of your application, design an appropriate schema for your application. 

* Q2.1 (15 points) Draw an ER diagram for this database. Make sure to indicate primary keys, cardinality constraints, weak entities (if any), and participation constraints. There might be extra constraints which cannot be captured by the E/R diagram, make sure you mention them below the diagram. List any assumptions you make in the process.

    Hint: The E/R diagram should contain ~10 (may be more/less) entities. You can see an E/R diagram example in the project description. Please do not copy it, create your own with your creativity.

* Q2.2 (15 points) For each entity set and relationship, write a short description in plain English of what it represents or models. One or two sentences per entity set and relationship is enough. These descriptions are primarily to help us understand that you are modeling your application correctly.

Common Mistakes to avoid in design:

1. Modeling a database administrator explicitly in your E/R diagram. The DBMS usually has its own internal representation for administrators.
2. Missing arrows or rounded arrows in a many-one and/or a one-one relationship.
3. Missing arrows from a weak set to the set(s) that provide its key attribute(s).
4. Using inheritance when there is no "ISA" connection between two sets.
5. Forgetting that when entity set B inherits from entity set A, B inherits
set A, B inherits everything that A has. In addition, B can define its own attributes of its own. Therefore, there is no need to repeat all the attributes/relationships that A has again for B.
6. "Cooking up" multi-way relationships, weak entity sets, or inheritance when they are not needed.
7. Forgetting to underline key attributes in the E/R model.
8. Repeating (reusing) names for different entity sets or for different relationships within
the same entity set, i.e., using the same name to denote two different things.
9. When converting a multiway relationship to many two-way relationships using a
connecting entity set, forgetting to introduce many-one relationships!

## Q3. SQL statements and presentation slides [30 points]

* Q3.1 (20 points) Translate the ER diagram into relational database tables (i.e. give the SQL DDL statements). Make sure that the translation captures key constraints (primary keys and foreign keys if applicable) and participation constraints in the ER diagram. Identify constraints, if any, that you are not able to capture. Create SQL scripts to create the database tables and populate your database with sample data. Include at least for each relation.

    Make sure you:
    * define data types correctly for each column
    * set null/optional constraints for each column
    * correctly define primary key and unique constraints (multiple unique constraints should be annotated with a label)
    * correctly define foreign key constraints
    * identify any requirements that it is not possible to model

    Note: We all know code style is important, so does SQL Style. See [SQL Style Guide](https://www.sqlstyle.guide/#white-space). 

* Q3.2 (10 points) 
    * Prepare a 4 minutes presentation slides in a powerpoint or pdf format
    * Present your project on 03/09 class

## Project GitHub Repository

Your project GitHub repository should, at a minimum, have the following directory structures and files:

* diagrams/ - a directory containing all model diagrams
* sql/install.sql - a file containing the SQL necessary to create the database schema
* sql/load.sql - a file containing the SQL necessary to load your schema with `sample` data
* slides/interimreport.pptx - your interim presentation file

Note: See the demo project for a potential starting point: https://github.com/yinlinchen/SuperHeros

## The tangible steps you will take for project assignment 2 are:
* Read and select the project.
* Understand the dataset.
* Create personas for your application.
* Model the database using an Entity-Relationship (ER) diagram.
* Design a relational database to store the dataset data.
    * Add primary and foreign key constraints.
    * Create database indexes.
    * ...
* Load sample data into the database.
* Think some questions and write (simple) advanced SQL queries to answer the questions.
* Prepare documentations:
    * Application specifications (Q1)
    * Designing the database (Q2)
    * SQL statements and presentation slides (Q3)
* Assemble all your works and put into your team project GitHub repository.
* Present a 4 mintues presentation about your project.

## Submitting your work
One (and only one) team member should submit for the team. The submission should contain the ssh URL for your team's git repository and the commit hash you wish to submit for grading.

The commit hash can be obtained by one of the following methods:
* use the "git log" command at the command line
* browse to your project in `github.com/<your github account>/<projectname>` and click on the repository's Commits.  You will see a list of commits along with the hash. 

Sumbit GitHub commit hash URL to `Project 2` in the Canvas.
1. GitHub commit hash URL. e.g. `https://github.com/<your github account>/cs4604-<groupname>/tree/5542903eb2e3a262a5ab32282997fde9fcb17c9e`

## Bonus points
You will grade other teams according to their presentations. E.g., If your team's project is `FilmFanatic`, then you will grade `TooManyGames` and `TravelLover` teams' presentations.

Three teams with the highest score will receive a 10 bonus points for project assignment 2.

## Reference
* [SQL Style Guide](https://www.sqlstyle.guide/#white-space)
