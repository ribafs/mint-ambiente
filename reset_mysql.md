## Resetando a senha de root do MySQL no Mint 19.3

```bash
sudo mysql -uroot
USE mysql;
UPDATE user SET plugin='mysql_native_password' WHERE User='root';
UPDATE user SET authentication_string=PASSWORD("root") WHERE User='root';
FLUSH PRIVILEGES;
exit;

sudo /etc/init.d/mysql restart

mysql -uroot -proot
```

