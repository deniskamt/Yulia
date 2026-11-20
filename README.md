# Демидовский Невьянск и деревянная Синячиха

Статический сайт экскурсии. Страница лежит в `public/index.html` (картинки
встроены в неё), раздаёт её `server.js` (Node.js, без зависимостей).

## Локальный запуск

```bash
npm start          # http://localhost:3000
```

## Деплой на Railway

1. railway.com → **New Project → Deploy from GitHub repo** → `deniskamt/Yulia`.
2. Railway сам определит Node.js-проект и запустит `node server.js`
   (настройки в `railway.json`, проверка работоспособности по `/health`).
3. Settings → Networking → **Generate Domain**, чтобы получить публичный адрес.

Переменные окружения не нужны: порт Railway передаёт сам через `PORT`.
