Configuração do php e apache

Configurar php

display_errors = On

sudo nano /etc/php/7.2/apache2/php.ini

Configurar apache

ServerName localhost

Trocando None por All

```bash
<Directory />
    Options Indexes FollowSymLinks Includes ExecCGI
    AllowOverride All
    Order deny,allow
    Allow from all
</Directory>
```

sudo nano /etc/apache2/apache2.conf

sudo systemctl restart apache2

Instalar adminer.php - http://adminer.org


