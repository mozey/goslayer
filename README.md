# goslayer

Inspired by [dbslayer](https://github.com/mozey/dbslayer)

## Design goals

### Ad-hoc SQL queries

Send SQL queries over HTTPS, get a JSON response

Supports reading and writing

### Row level security

Auth with row level security using [JWT](https://jwt.io/)

Creates "hidden" tables to manage users, roles, and groups if required, with interface to use external system for auth instead

### Parses SQL

SQL queries are parsed and validated before they are sent to the DB engine

[sqlc](https://github.com/kyleconroy/sqlc) supports parsing
- SQLite
- PostgreSQL
- MySQL

[sqlparser](https://github.com/xwb1989/sqlparser)
- MySQL

Others?


