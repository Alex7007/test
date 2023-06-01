# Используем образ PHP
FROM php:latest

# Устанавливаем зависимости
RUN apt-get update && apt-get install -y \
    libpq-dev \
    && docker-php-ext-install pdo_mysql

# Копируем код приложения
COPY . /var/www/backend

# Устанавливаем рабочую директорию
WORKDIR /var/www/backend

# Запускаем приложение при старте контейнера
CMD ["php", "-S", "0.0.0.0:80"]