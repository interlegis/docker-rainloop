# docker-rainloop

A minimalistic docker version of [Rainloop Community Edition](http://www.rainloop.net/)

## Quickstart

To Start the container use the following command.

```
docker run -d -p "80:80" solidnerd/rainloop
```

**or**

```
docker-compose up
```

use [docker-compose](https://github.com/docker/compose) .

## Save the Rainloop data persistent
If you want the Rainloop data persistent than use the exposed Volume with a command like this:
```
docker run -d -p "80:80" -v $(pwd)/data:/var/www/rainloop/data solidnerd/rainloop
```

## Rainloop Specifica

### Contacts
This container supports all Database PHP extensions for the contacts:
- MySQL
- PostgreSQL
- SQLite

### Versions
Using the standard edition instead of the community edition is possible aswell. To do that you need to change [RAINLOOP_VERSION](https://github.com/SolidNerd/docker-rainloop/blob/master/Dockerfile#L5) to `RAINLOOP_VERSION http://repository.rainloop.net/v2/webmail/rainloop-latest.zip`.


# LICENSE
The MIT License (MIT)

Copyright (c) 2016 Niclas Mietz