# Matomo-docker

Matomo docker compose files.

It starts the following services:
* db - Mariadb
* app - Matomo analytics
* anubis - Http request scanner to protect from scraper bots
* web - Nginx reverse proxy

## .env example

```bash
MYSQL_PASSWORD=changeme
MYSQL_DATABASE=matomo
MYSQL_USER=matomo
ANUBIS_VERSION=version
ANUBIS_TARGET_INSECURE_SKIP_VERIFY=true
NGINX_VERSION=version
MATOMO_VERSION=version
MATOMO_DATABASE_HOST=db
MATOMO_DATABASE_ADAPTER=mysql
MATOMO_DATABASE_TABLES_PREFIX=matomo_
MATOMO_DATABASE_USERNAME=matomo
MATOMO_DATABASE_PASSWORD=changeme
MATOMO_DATABASE_DBNAME=matomo
MARIADB_VERSION=version
MARIADB_AUTO_UPGRADE=1
MARIADB_DISABLE_UPGRADE_BACKUP=1
MARIADB_INITDB_SKIP_TZINFO=1
MARIADB_ROOT_PASSWORD=changeme
```
