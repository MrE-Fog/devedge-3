## iPhone Umleitung mit einer .htaccess-Datei

```apache_conf
Options +FollowSymlinks
RewriteEngine On

RewriteCond %{HTTP_USER_AGENT} ^.*iPhone.*$
RewriteRule ^(.*)$ http://iphone.domain.de [R=301]
```
