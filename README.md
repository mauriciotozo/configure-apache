# configure-apache

sudo a2enmod vhost_alias

## Exemplo de vhost

```
<VirtualHost *:80>
    ServerName dev.lab
    ServerAlias *.lab

    VirtualDocumentRoot /var/www/html/%1.0/public

    ErrorLog /var/log/apache2/error-virtual.log
    CustomLog /var/log/apache2/access-virtual.log combined

    LogLevel warn
</VirtualHost>
```
