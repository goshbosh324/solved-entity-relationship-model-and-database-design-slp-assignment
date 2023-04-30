Download Link: https://assignmentchef.com/product/solved-entity-relationship-model-and-database-design-slp-assignment
<br>
5/5 - (2 votes)

Module 2 – SLP

Entity-Relationship Model and Database DesignSLP Assignment

Improving Database Design Through Entity-Relationship Modeling

The purpose of this SLP assignment is to refine database design using ER modeling principles. You are required to continue working on the project started in the previous SLP and do the following:

1.    Identify all relevant entities and relationships.

2.    Use ER diagrams to present them.

When you have finished, place them into a Word document.

SLP Assignment Expectations

·         Improve existing database design using entity-relationship modeling methods.

·         Communicate effectively with your audience.

Module Overview

In the previous module, we introduced the concepts for the relational data model, including data model, relation, schema, attribute, key, and relation instance.

This module will introduce the basic entity-relationship (ER) data model and rules for designing a good ER model.

Module 2 – BackgroundEntity-Relationship Model and Database DesignData Modeling is the process of creating a data model for a given set of data, and it is a major part in software development. The way data is modeled is very important for how it can be accessed and manipulated using SQL.

The dominant design methodology for relational databases consists of three steps:

1.    Identify all relevant entities and relationships, and describe them using ER diagrams.

2.    Convert the ER model to a number of relation schemas.

3.    Eliminate (or reduce) redundancy by splitting relations. This process is called normalization.

In most cases, an entity can be identified uniquely in its entity set by the values of its attributes. A relationship in the ER model is exactly the relation in the relational data model.

·         Entity sets correspond to the domains of the values.

·         Tuples correspond to connections between entities.

·         Relationship instances form a table, like relation instances.

In our Books example from Module 1, books and authors are two entity sets. Each tuple (book, author) corresponds to a connection between two specific entities in the sets. Books and their author relationships form the table below.

BooksAuthorsThe Lost SymbolDan BrownSuperfreakonomicsSteven Levitt and Stephen DubnerLego Star WarsSimon Beecroft……Good data modeling can be difficult because there may be many data models to choose from. The following design principles can be useful when considering a design:

·         Be faithful to the specification of the application.

·         Avoid duplication and other redundant information.

·         The KISS principle (Keep It Simple, Stupid).

·         Choose the right relationship.

·         Use attributes when possible.

Read through the slides for Module 2, and make sure you understand the core concepts introduced there, mainly the entity relationship diagram and its components: entities, attributes, and relationships.

Common Database Design MistakesNeophyte database designers (and professionals, on occasion) are prone to several common mistakes. Here’s a checklist to ensure that you haven’t made any of the most common database design errors.

1.    Spreadsheet design. If you need a spreadsheet, use a spreadsheet. Your database shouldn’t be a single table of all sorts of business data, especially if it included a number of calculated values. Combining different types of data in one table defeats the whole purpose of using a relational database. And while storing calculated values can speed up query and report performance, databases generally calculate values on the fly so the data is always as current as possible.

2.    Too much data. The goal of a successfully designed database is to provide all of the information necessary for making decisions based on the data. There is an overwhelming desire, especially in neophytes, to encapsulate every possible nugget of data in the database. Too many fields in an entry form guarantee users will lose interest in filling in the data or will increase the amount of time to fill out the form. Plus this information increases the overall storage requirements for the database. Proper research can help identify what is essential, what might be useful in the future, and what is irrelevant.

3.    Compound fields. Fields containing multiple discrete pieces of data lead to problems in searching, alphabetizing, and calculating those fields. It’s much harder to get a report of customers by ZIP code when that value is buried in a field with the address, city, and state. If it’s a distinct piece of data, make it a distinct field.

4.    Missing keys. Every table needs some sort of key to identify individual records. Most database packages alert you if you leave one out during the design process, but if you use your own system (such as a flat file system), make sure there is a distinct and unique key for each record in each table.

5.    Bad keys. A key has to be unique for each record. Existing database fields may appear to be good candidates for keys, but it is usually best to create an artificial key that is guaranteed to be unique. Phone numbers seem like a great key for personnel records until you run into people who live in the same home or who have multiple phone lines.

6.    Missing relations. If two tables are supposed to be related, there must be a field that relates the two databases. A well-designed table relationship is useless if the appropriate foreign keys are not added to the related tables (or if the linking table for a many-to-many relationship is not created).

7.    Unnecessary relationships. Just because every table can be linked to every other table does not mean that they have to be related. There is a temptation to relate tables that are logically unrelated just because you can.

8.    Incorrect relations. Creating relationships between tables does not require changes in each table. A one-to-many relationship requires the primary key from the “one” table to be inserted as a foreign key in the “many” table. It does not need a foreign key placed in the “one” table since the relationship is already established in the “many” table. In fact, this arrangement may yield incorrect query results.

9.    Duplicate field names. DBMS products prevent duplicate field names in a single table, but do not prevent duplicate names in different tables. While there is no programmatic reason to follow this practice, it becomes very difficult for humans to keep track of 15 relational tables where the primary key in each is called ID. It is much easier to write and debug queries if each field name is unique in the entire database.

10.  Cryptic field and table names. Even more frustrating than duplicate names are cryptic names. There is no reason to limit the length of a field or table name, so use as descriptive a name as possible. Writing queries and debugging are much easier when the focus is the logic and not what “T1C1x” means.

11.  Missing or incorrect business rules. Many businesses have strict rules that have nothing to do with program or database logic. Do not neglect these rules. The old adage of “garbage in, garbage out” applies since decisions made on incorrectly entered data may lead to erroneous query results and reporting.

12.  Missing or incorrect constraints. A very easy way to ensure that data are entered correctly is to use constraints. These can be implemented as checks to see if an entered value is within an approved list or range of choices. Constraints can also be implemented as masks that require phone numbers or ZIP codes to fit a specified format.

13.  Referential integrity. Data records that participate in relationships need to be checked when they are created or deleted to ensure that they are not orphans. Deleting one record usually requires the deletion of that record in linked tables. Ensuring referential integrity involves making sure that table declarations ensure the existence of the appropriate relationships and that integrity checks are triggered when records are deleted.

14.  Database security. Almost all databases have methods to control access and user rights. For instance, end users of an invoice system probably should not have permission to create new tables or delete existing tables. Use the available security features to prevent unauthorized access and control permissions of various users and classes of users.

15.  International issues. As business becomes more global, keep in mind that there are a number of formats for business data other than those of the United States. Most databases understand the various European and American date, currency, and address formats so think about whether your application will need to understand those as well.

Required Reading·         PowerPoint Presentation: Entity-Relationship Model and Database Design

·         Allen, S. and Terry, E. (2005), Beginning Relational Data Modeling, Chapter 3 – Understanding Relational Modeling Terminology (read the remaining sections from Relationships), or from <a href="http://books.google.com/books?id=62CFtFea0NsC&amp;printsec=frontcover&amp;source=gbs_v2_summary_r&amp;cad=0#v=onepage&amp;q=&amp;f=false" target="_blank" rel="nofollow noopener">http://books.google.com/books?id=62CFtFea0NsC&amp;printsec=frontcover&amp;source=gbs_v2_summary_r&amp;cad=0#v=onepage&amp;q=&amp;f=false</a>.

·         Allen, S. and Terry, E. (2005), Beginning Relational Data Modeling, Chapter 4: Understanding Data Modeling Methods: Graphical Syntax, or from <a href="http://books.google.com/books?id=62CFtFea0NsC&amp;printsec=frontcover&amp;source=gbs_v2_summary_r&amp;cad=0#v=onepage&amp;q=&amp;f=false" target="_blank" rel="nofollow noopener">http://books.google.com/books?id=62CFtFea0NsC&amp;printsec=frontcover&amp;source=gbs_v2_summary_r&amp;cad=0#v=onepage&amp;q=&amp;f=false</a>.

·         Relational Database Design Requirements, <a href="http://www.databasedev.co.uk/database_design_requirements.html" target="_blank" rel="nofollow noopener">http://www.databasedev.co.uk/database_design_requirements.html</a>