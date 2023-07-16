# Create laravel project

`docker compose run laravel composer create-project laravel/laravel /var/www`

# Run commands in laravel container

Run a command in the laravel container, for example adding a composer package.

`docker compose run laravel composer require owen-it/laravel-auditing`

--

Good luck!

# Configuration

Here are the defaults which can always be updatd in the `dcoerk-compose.yml` file.

## Mailhog

```
SMTP: mailhog
Port: 1025
HTTP UI: localhost:8025
```

## Redis

No password.

```
Host: cache
Port: 6379
```

## PostreSQL Database

```
Host: db
User: root
Password: password
Port: 5432
```

## NGINX

Web app available at `localhost:8000`
