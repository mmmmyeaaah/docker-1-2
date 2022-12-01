Сборка образа

docker build ./ --tag stockproducts

Запуск контейнера

docker run --name stockproducts -d -p 8000:8765 stockproducts
