# Tutorial: Accessing a relational database

This tutorial introduces the basics of accessing a relational database with Go and the `database/sql` package in its standard library. You’ll get the most out of this tutorial if you have a basic familiarity with Go and its tooling. If this is your first exposure to Go, please see [Tutorial: Get started with Go](/doc/tutorial/getting-started) for a quick introduction.

The `database/sql` package you’ll be using includes types and functions for connecting to databases, executing transactions, canceling an operation in progress, and more. For more details on using the package, see [Accessing databases](/doc/database/index).

In this tutorial, you’ll create a database, then write code to access the database. Your example project will be a repository of data about vintage jazz records.

In this tutorial, you’ll progress through the following sections:

1. Create a folder for your code.
2. Set up a database.
3. Import the database driver.
4. Get a database handle and connect.
5. Query for multiple rows.
6. Query for a single row.
7. Add data.

**Note:** For other tutorials, see [Tutorials](https://go.dev/doc/tutorial/index.html).

### Running MySQL for local development

```bash
./start_mysql.sh
```

The server will be available at `localhost:3306`

To connect to the MySQL database in another terminal, enter:

```bash
docker exec -it mysql mysql -uroot -pmysql
mysql> use mysql;
```