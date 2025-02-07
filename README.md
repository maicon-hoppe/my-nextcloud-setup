# my-nextcloud-setup

A setup script with docker compose for nextcloud with onlyoffice.

Is necessary to add this line to crontab, so nextcloud common tasks can be performed with CRON:

```
*/5  *  *  *  * docker exec -u www-data nextcloud php -f /var/www/html/cron.php
```
