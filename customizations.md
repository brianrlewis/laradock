# My Customizations

## Environment Variables (.env.example)

`WORKSPACE_INSTALL_MYSQL_CLIENT=true`
`PHP_VERSION=8.0`

## Enable HTTPS

Open `laradock/nginx/sites/default.conf` and uncomment the HTTPS section

## Enable Horizon

`cd laravel-horizon/supervisord.d`
`cp laravel-horizon.conf.example laravel-horizon.conf`
Update `laravel-horizon/supervisord.d/.gitignore` to exempt conf file

## Enable Scheduler

`cd php-worker/supervisord.d`
`cp laravel-scheduler.conf.example laravel-scheduler.conf`
Update `php-worker/supervisord.d/.gitignore` to exempt conf file
