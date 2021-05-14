127.0.0.1       berletek.tornazzvelem.docker

docker-compose up -d --build

docker-compose exec php composer install

docker-compose exec php /app/bin/console doctrine:query:sql "select 1;"

docker-compose run --rm nodejs gulp
docker-compose run --rm nodejs gulp vendor

docker-compose logs -f 