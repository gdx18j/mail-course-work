# Курсовая работа: Почтовый сервер с безопасным обменом

## Установка и запуск

1. Установите Docker и Docker Compose
2. Скачайте проект: git clone https://github.com/gdx18j/mail-course-work.git
3. Запустите: docker-compose up -d
4. Создайте пользователя: docker exec mail-server setup email add user@course.local --password 1234

## Доступ к сервисам

- Почта: http://localhost:8888 (user@course.local / 1234)
- Управление БД: http://localhost:8080 (admin@example.com / admin)
- Мониторинг: http://localhost:9000

## Безопасность

- SSL/TLS шифрование на портах 993 (IMAP) и 465 (SMTP)
- Антиспам фильтрация (Rspamd)
- Защита от атак (Fail2ban)
