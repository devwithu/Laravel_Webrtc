- sudo chgrp -R www-data storage bootstrap/cache
- sudo chmod -R ug+rwx storage bootstrap/cache

- sudo find . -type f -exec chmod 664 {} \\;
- sudo find . -type d -exec chmod 775 {} \\;

- cp .env.real .env
- composer install

- mysql -u tabbada -p -h 127.0.0.1 tabbada < tabbada.sql

