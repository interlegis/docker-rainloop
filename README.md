# docker-rainloop

A minimalistic docker version of [Rainloop Community Edition](http://www.rainloop.net/)

## Version: [1.12.1](http://www.rainloop.net/changelog/)

## Quickstart

To Start the container use the following command.

```
docker run -d -p "80:80" interlegis/alpine-rainloop:1.12.1
```

**or**

```
docker-compose up
```

use [docker-compose](https://github.com/docker/compose) .

## Save the Rainloop data persistent
If you want the Rainloop data persistent than use the exposed Volume with a command like this:
```
docker run -d -p "80:80" -v $(pwd)/data:/var/www/rainloop/data interlegis/alpine-rainloop:1.12.1
```

## Rainloop Specifica

### Contacts
This container supports all Database PHP extensions for the contacts:
- MySQL
- PostgreSQL
- SQLite


# LICENSE
The MIT License (MIT)

Copyright (c) 2016 Niclas Mietz
Updated to 1.12.1 by Interlegis (2018)
