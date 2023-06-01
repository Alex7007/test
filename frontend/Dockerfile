# Используем образ Node.js
FROM node:latest

# Копируем код приложения
COPY . /var/www/frontend

# Устанавливаем рабочую директорию
WORKDIR /var/www/frontend

# Устанавливаем зависимости и собираем фронтенд
RUN npm install && npm run build

# Запускаем приложение при старте контейнера
CMD ["npm", "start"]