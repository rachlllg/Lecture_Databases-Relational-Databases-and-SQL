## The lectures and exercises are based on StandfordOnline course 'Databases: Relational Databases and SQL'.


### SQLite Installation:
Download the Precompiled Binaries for MacOS
https://www.sqlite.org/download.html

### Basic SQLite Operations:
Navigate to the folder you wish to work on and run: sqlite3
https://www.sqlite.org/cli.html

--> to create a new schema/table with various attributes/columns
sqlite> CREATE TABLE table_name (
        attribute_1_name attribute_1_type PRIMARY KEY,
        attribute_2_name attribute_2_type,
        ...);

--> to insert new tuples/rows into each attribute in the new schema
sqlite> INSERT INTO table_name VALUES (attribute_1, attribute_2, ...);

--> to remove a row from a schema
sqlite> DELETE FROM table_name WHERE column_name = 'condition';

--> to show all schemas
sqlite> .schema

--> to show the content of a schema in table format
sqlite> .headers on
sqlite> .mode columns
sqlite> SELECT * FROM table_name;

--> to remove a schema
sqlite> DROP TABLE table_name;

--> to create/open a new database
sqlite> .open new_db.db

--> to run the SQLite commands in a .sql file
sqlite> .read schema_name.sql

---> to exit in the middle of a sqlite query
sqlite> control+D
