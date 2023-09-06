### Xdebug Setup Steps:

Xdebug Wizard URL: https://xdebug.org/wizard

1. Download xdebug file -> cut -> paste to xampp->php->ext

2. Copy the below code and paste under your php.ini file

```
xdebug.mode=debug
xdebug.start_with_request=trigger
xdebug.client_port=9003
xdebug.client_host = localhost
zend_extension="C:\xampp\php\ext\xdebug.dll"
```

3. Install PHP Debug extention your visual studio code.

*Always turn on your XAMPP
*You must put your file on XAMPP htdocs
