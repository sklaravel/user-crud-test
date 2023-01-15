<p align="center"><a href="https://spadeinfotech.net/" target="_blank"><img src="https://spadeinfotech.net/wp-content/uploads/2020/07/SI6.png" width="649" height="165" alt="Spade Logo"></a></p>

## Resources used

- Laravel version 9.40.1
- PHP version 8.1.6
- Apache/2.4.53 (Win64) OpenSSL/1.1.1n
- Database client version: libmysql - mysqlnd 8.1.6
- Server version: 10.4.24-MariaDB [MySQL 8] - <a href="https://mariadb.com/kb/en/mariadb-vs-mysql-compatibility/" target="_blank">mariadb.org binary distribution</a>

## Apache setup
```
<VirtualHost *:80>
    ServerName spade.zz
    DocumentRoot "F:/user-crud-test/public"
    SetEnv APPLICATION_ENV "development"
    <Directory "F:/user-crud-test/public">
        Options Indexes FollowSymLinks MultiViews
        AllowOverride all
        Order Deny,Allow
        Allow from all
        Require all granted
    </Directory>
</VirtualHost>
```
