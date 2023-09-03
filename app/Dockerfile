# Используйте официальный образ Python
FROM python:3.8-slim

# Устанавливаем директорию приложения в контейнере
WORKDIR /app

# Копируем файлы приложения в контейнер
COPY myapp1.py /app/
#COPY index.html /app/

# Установка необходимых зависимостей
#RUN pip install http.server

# Установка curl
RUN apt-get update && apt-get install -y curl

# Устанавливаем необходимые переменные окружения
ENV AUTHOR="RolanAR"
ENV UUID="69357461-cc16-4eb3-8f3b-374d141d9b1c"

# Указываем, что контейнер слушает порт 8000
EXPOSE 8000

# Запускаем ваше приложение
CMD ["python3", "myapp1.py"]

