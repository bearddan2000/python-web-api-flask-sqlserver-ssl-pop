# python-web-api-flask-sqlserver-ssl-pop

## Description
Creates an api of pop for a flask project.
Has the ability to query by parameters.
If path is not found, will default to 404 error.

Sql server uses self-signed ssl.

## Tech stack
- python
- flask

## Docker stack
- alpine:edge
- python:latest
- mcr.microsoft.com/mssql/server:2017-CU17-ubuntu

## To run
`sudo ./install.sh -u`
- Get all pops: http://localhost/pop
  - Schema id, name, and color
- Query with params: http://localhost/pop <id>

## To stop (optional)
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- https://stackabuse.com/using-sqlalchemy-with-flask-and-postgresql/
- https://stackoverflow.com/questions/27766794/switching-from-sqlite-to-mysql-with-flask-sqlalchemy
