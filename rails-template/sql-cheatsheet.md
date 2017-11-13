### Common SQL Commands
* CREATE DATABASE database_name; # From the $USER database.
* CREATE TABLE table_name (id serial PRIMARY KEY, some_column varchar, another_column int, yet_another_column timestamp);
* ALTER TABLE table_name ADD column_name boolean;
* ALTER TABLE table_name DROP column_name;
* INSERT INTO contacts (name, age, birthday) VALUES ('Wes', 43, '1969-05-01') RETURNING id;
* SELECT * FROM table_name WHERE age >= 18;
* SELECT * FROM contacts WHERE NOT age >= 18;
* UPDATE contacts SET name = 'Wes Anderson' WHERE id = 1;
* DELETE FROM contacts WHERE id = 1;
* DROP TABLE table_name; # From the database that holds the table.
* DROP DATABASE test_database; # From the $USER database.
### Common psql Commands
* List all databases: \l
* Connect to database: \c database_name
* List tables in current database: \dt
* List columns in a table: \d table_name
* Exit out of help menu: \q
* See a list of all psql commands: \? (Press the down arrow to scroll through, or q to exit list.)
### Common Terminal Commands
* `$ psql` to launch psql.
* `$ postgres` to launch postgres.
* CMD + T (or Terminal > Shell > New Tab from menu options) to open a new tab in the Terminal. This allows you to run postgres and psql at the same time in a single terminal window.
### Common Column Types
* int
* float
* varchar
* text (for long strings of text)
* timestamp
* boolean
### Operators for WHERE clauses
* `=`
* `!=`
* `>`
* `<`
* `>=`
* `<=`
* `BETWEEN`
* `LIKE`
* `IN`
