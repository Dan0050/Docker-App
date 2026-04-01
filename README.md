# First Docker app

Простое веб-приложение на nginx в Docker-контейнере.


### Запуск
docker build -t myapp:1.0 .
docker run -d -p 8080:80 myapp:1.0
