Сборка образа

docker build ./ --tag stockproducts

Запуск контейнера

docker run --name stockproducts -d -p 8765:8000 stockproducts
