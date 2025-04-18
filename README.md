<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

## Laravel 11 Docker
- Laravel v11
- PHP v8.3
- MySQL v8.1
- phpMyAdmin v5
- Mailpit v1

##  How To Deploy
- `git clone https://github.com/SutoIstvan/laravel-11-docker.git`
- `cd laravel-11-docker`
- `rename .env.example to .env`
- `docker compose up -d --build`
- `docker compose exec phpmyadmin chmod 777 /sessions`
- `docker compose exec php bash`
- `chown -R www-data:www-data /var/www/storage /var/www/bootstrap/cache`
- `chmod -R 775 /var/www/storage /var/www/bootstrap/cache`
- `composer install`
- `php artisan key:generate`

## Laravel App
- URL: http://localhost

## Mailpit
- URL: http://localhost:8025
## phpMyAdmin
- URL: http://localhost:8080
