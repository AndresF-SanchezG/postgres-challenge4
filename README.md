# Periodic Table Database

This code snippet is a PostgreSQL database dump in SQL format. It represents a series of SQL statements that, when executed in a PostgreSQL database, will recreate the structure of the database and populate it with sample data. Here's a breakdown of the code:

Initial Setup:

Various settings related to timeouts, encoding, and configurations are established.
The existing "periodic_table" database is dropped if it already exists.
A new database named "periodic_table" is created using "template0" as the template, with specified encoding and locale settings.
Connecting to the New Database:

The script connects to the "periodic_table" database to perform further operations.
Table Creation:

Three tables are created in the "public" schema: "elements," "properties," and "types."
Each table has specific columns to store data related to chemical elements and their properties.
Sequence Creation:

A sequence is created to generate primary key values for the "types" table.
Associating Sequence with Primary Key:

The sequence created earlier is assigned as the default value generator for the "type_id" column in the "types" table.
Inserting Sample Data:

Example records are inserted into the "elements," "properties," and "types" tables using INSERT INTO statements.
Adjusting Sequence Value:

The current value of the sequence for "types" is set to align with the last inserted record.
Defining Constraints:

Unique constraints and primary key constraints are defined for columns in the "elements," "properties," and "types" tables.
Foreign key constraints are defined to maintain referential integrity between the "properties" table and the "elements" and "types" tables.
Database Dump Completion:

The database dump process is completed.
In summary, this code creates a PostgreSQL database named "periodic_table" with three tables: "elements," "properties," and "types." It inserts sample data into these tables and establishes constraints and relationships between them. The dump can be used to recreate the database structure and data in a PostgreSQL environment.


# Screenshot

### Elements Table
![Captura1](https://github.com/AndresF-SanchezG/postgres-challenge4/assets/113924667/361fb2d3-4d09-4fc0-b21b-76f971fc9a69)

### Elements Table
![Captura2](https://github.com/AndresF-SanchezG/postgres-challenge4/assets/113924667/9b8a87d4-7a2a-46a3-9cc6-a4c8b212fb3e)

### Properties Table
![Captura4](https://github.com/AndresF-SanchezG/postgres-challenge4/assets/113924667/0bd6045c-6d39-47f8-8617-11ce667e6956)

### Run with Arguments
![Captura7](https://github.com/AndresF-SanchezG/postgres-challenge4/assets/113924667/db801ddd-ef22-433d-87d4-bf5d3f2bad55)
![Captura8](https://github.com/AndresF-SanchezG/postgres-challenge4/assets/113924667/0e6b3b6d-3e99-4e51-a62c-e8c5f4161034)
![Captura9](https://github.com/AndresF-SanchezG/postgres-challenge4/assets/113924667/c32c6df6-2cfe-4b05-9bd2-fa479187f8b2)

# Author

- Autor - [@AndresF-SanchezG](https://github.com/AndresF-SanchezG)
- School - [Freecodecamp](https://www.freecodecamp.org/)
- Curse - [Build a Periodic Table Database](https://www.freecodecamp.org/learn/relational-database/build-a-periodic-table-database-project/build-a-periodic-table-database)
