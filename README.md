## Docker 

Простое веб-приложение на nginx в Docker-контейнер.


#### Сброка и Запуск
```bash
docker build -t myapp:1.0 .
docker run -d -p 8080:80 myapp:1.0
```
## Kubernetes Deployment
Образ загружен на Docker Hub
```docekr pull dan0050/docker-app```

#### Требования
```
minikube
kubectl
```
#### Запуск
```bash

# Применить все манифесты
kubectl apply -f k8s/

# Проверить поды
kubectl get pods

# Проверить сервисы
kubectl get services

# Получить доступ для Minikube
minikube service myapp-serv --url
