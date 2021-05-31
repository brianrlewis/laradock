# My Customizations

## Environment Variables (.env.example)

`WORKSPACE_INSTALL_MYSQL_CLIENT=true`
`PHP_VERSION=7.4`

## Enable HTTPS

Open the following file and uncomment the HTTPS section

laradock/nginx/sites/default.conf

## Enable Horizon

`cd laravel-horizon/supervisord.d`
`cp laravel-horizon.conf.example laravel-horizon.conf`

## Enable Scheduler

`cd php-worker/supervisord.d`
`cp laravel-scheduler.conf.example laravel-scheduler.conf`

# Startup Command

`docker-compose up nginx mysql redis laravel-horizon php-worker`
