# Technical 1
## DBA/Backend

There are two short questions.  That's right, you get to have twice the fun as the frontend developer.  :sunglasses:

### Question 1
Given these tables

gatekeeper_user | &nbsp; | &nbsp;
--------------- | - | -
id (primary key) | email (varchar) | belongs_to_circle_id (fk)

common_cirlces | &nbsp;
-------------- | - 
id (primary key) | name (varchar)


Write a sql query that fetches all unique email domains and counts them for circle name 'Retailer'.  Email data should be considered valid format.  e.g. 'john@example.com'

Expected Result format

domain | count
------ | ------
acme.com | 5
example.com | 10

### Question 2
TBD This will be a Python/Django problem.
