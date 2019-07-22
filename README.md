[![Build Status](https://travis-ci.org/ea1het/aws-ip.svg?branch=master)](https://travis-ci.org/ea1het/aws-ip)

# AWS IP
A microservice to capture, store and supervise AWS IPs 

## Backend storage
In order to make this piece of software to work you need a MariaDB/MySQL RDMS. Once you have it installed, please create the necessary tables described in [db_schema.txt](db_schema.txt). 

## Environment variables
This microservice uses environment variables in order to configure database access. This is a security measure to avoid leaving credentials hardcoded in software. 

In order to make this piece of software to work you need to either define environment variables yourself in your shell or create a file named `.env` beside the file [app.py](app.py). In both cases, the contents needed are this:

```
export DB_HOST="put_your_host_or_ip_here"
export DB_USER="here_cones_your_username"
export DB_PASS="here_comes_your_password"
export DB_TABL="put_here_database_table_name"
```
