# laravel todo app

TODO API using PHP and Docker

# set up

open your '.env' and add the following lines:

APP_PORT=8001
FORWARD_DB_PORT=5434

- install docker
- ./vendor/bin/sail up

NOTE: When you see commands like php artisan make:model Todo replace php with ./vendor/bin/sail. We don't have php installed locally, sail will use php within our Docker instance.

./vendor/bin/sail.artisan make:migration create_todos_table