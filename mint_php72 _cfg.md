## Configuração do php e apache

### Configurar php

sudo nano /etc/php/7.2/apache2/php.ini

display_errors = On



### Configurar apache

sudo nano /etc/apache2/apache2.conf

Adicionar

ServerName localhost

Trocar None por All

```bash
<Directory />
    Options Indexes FollowSymLinks Includes ExecCGI
    AllowOverride All
    Order deny,allow
    Allow from all
</Directory>
```
sudo systemctl restart apache2


### Sugestão: 

Instalar agerenciador web do MySQL adminer.php - http://adminer.org



