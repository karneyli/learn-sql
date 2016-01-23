# learn-sql
Project that has some dummy data for people to learn SQL using Heroku Dataclips

## Setup

Easy peasy.  

```bash
heroku run bash
psql $DATABASE_URL -f world.sql
```

## About world.sql

This is a standard sample database, found from http://pgfoundry.org/projects/dbsamples/


There seems to be three(3) tables:

### city

column_name    | data_type   | character_maximum_length
---            | ---         | ---
id             | integer     |
name           | text        |
countrycode    | character   | 3
district       | text        |
population     | integer     |

### country

column_name    | data_type   | character_maximum_length
---            | ---         | ---
code           | character   | 3
name           | text        |
continent      | text        |
region         | text        |
surfacearea    | real        |
indepyear      | smallint    |
population     | integer     |
lifeexpectancy | real        |
gnp            | numeric     |
gnpold         | numeric     |
localname      | text        |
governmentform | text        |
headofstate    | text        |
capital        | integer     |
code2          | character   | 2

### countrylanguage

column_name    | data_type   | character_maximum_length
---            | ---         | ---
countrycode    | character   | 3
language       | text        |
isofficial     | boolean     |
percentage     | real        | 
