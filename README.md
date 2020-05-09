# goslayer
Upbeat version of dbslayer, less metal

Design goals
- Ad hoc API, send SQL queries over HTTPS, get a JSON reponse
- Inspired by [dbslayer](https://github.com/mozey/dbslayer)
- Why bother learning GraphQL if you already know SQL?
- Additional auth in the go middleware or route handler


This is intended to be useful as a supplimentary route on existing APIs, think about
- restricting ad hoc qeuries to specific db users or views
- or adding filters to the add hoc query, e.g. the authenticated user is only authorized to view rows where col x = value y
- only allow known query types by parsing query SQL 

