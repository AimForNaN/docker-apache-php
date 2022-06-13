# docker-apache-php

Configured to also parse HTML files through PHP.

## Volumes

> Adjust volumes before building to customize.

| Source | Target |
| ------ | ------ |
| ./www  | /var/www |
| ./conf/vhosts | /etc/apache2/sites-enabled |
| ./logs/httpd | /var/log/apache2 |

## Default Virtual Host

> Adjust default or use it as a reference for new virtual hosts.

| Host | Document Root | Config |
| ---- | ------------- | ------ |
| localhost:8080 | /var/www/html | ./conf/vhosts/site.conf |

> Can be adjusted post-build.

## Build

```console
docker-compose up --build
```
