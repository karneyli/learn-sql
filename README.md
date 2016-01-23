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

### countrylanguage


