запуск приложеня
pyton3 myapp1.py

проверка работоспособности
Для получения имени хоста:
curl http://localhost:8000/hostname
Для получения значения $AUTHOR:
curl http://localhost:8000/author
Для получения значения $UUID:
Copy code
curl http://localhost:8000/id

Docker

docker build -t rolan777/myapp1-image .

docker run -d -p 8000:8000 rolan777/myapp1-image

docker ps

проверка работоспособности

docker stop CONTAINER ID

docker login

docker push rolan777/myapp1-image

