
# Обновление клиента PostgreSQL в Konga

## Изменения

1. Обновлен драйвер PostgreSQL с `sails-postgresql@0.11.4` до `sails-postgresql@5.0.0`, что обеспечивает поддержку PostgreSQL 15/16
2. Заменен устаревший `node-sass` на современный `sass` (Dart Sass) для совместимости с актуальными версиями Node.js
3. Обновлены зависимости для обеспечения работы с внешними базами данных

## Настройка подключения к облачному кластеру PostgreSQL

Для подключения к внешнему/облачному кластеру PostgreSQL используйте следующие переменные окружения:

```bash
DB_ADAPTER=postgres
DB_HOST=ваш-хост-кластера
DB_PORT=5432
DB_USER=ваш-пользователь
DB_PASSWORD=ваш-пароль
DB_DATABASE=ваша-база-данных
DB_SSL=true
```

## Совместимость

- Поддержка PostgreSQL 15 и 16
- Совместимость с Node.js 18+
- Поддержка подключения к облачным кластерам PostgreSQL (AWS RDS, Google Cloud SQL, Azure Database и др.)

## Установка

```bash
npm install
npm start
```
