# laravel-couchdb-boilerplate



git clone https://github.com/robsonvn/laravel-couchdb-boilerplate.git


cd laravel-couchdb-boilerplate
composer install

chmod -R 775 storage && chmod -R 775 bootstrap/cache

cp .env.example .env

php artisan key:generate && php artisan cache:clear

curl -X PUT http://localhost:5984/laravel-database
