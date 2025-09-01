# Matomo-docker

Matomo docker compose files.

It starts the following services:
* db - Mariadb
* app - Matomo analytics
* anubis - Http request scanner to protect from scraper bots
* web - Nginx reverse proxy
* cert - Certbot to request/renew certificates from [letsencrypt](https://letsencrypt.org/)
* wt - Watchtower to automatically update to new versions of docker images

## Variables .env file

Example:

```bash
MYSQL_PASSWORD=changeme
MYSQL_DATABASE=matomo
MYSQL_USER=matomo
ANUBIS_VERSION=1.21.3
ANUBIS_TARGET_INSECURE_SKIP_VERIFY=true
MATOMO_VERSION=5.4.0
MATOMO_DATABASE_HOST=db
MATOMO_DATABASE_ADAPTER=mysql
MATOMO_DATABASE_TABLES_PREFIX=matomo_
MATOMO_DATABASE_USERNAME=matomo
MATOMO_DATABASE_PASSWORD=changeme
MATOMO_DATABASE_DBNAME=matomo
MARIADB_AUTO_UPGRADE=1
MARIADB_DISABLE_UPGRADE_BACKUP=1
MARIADB_INITDB_SKIP_TZINFO=1
MARIADB_ROOT_PASSWORD=changeme
```
