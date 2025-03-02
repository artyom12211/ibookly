Создай в новом проекте директории /frontend и /backend

## Общее
`npm i -G pnpm`

## Фронтенд:
[ibookly-frontend](https://github.com/artyom12211/ibookly-client)\n
cd /frontend\n
git clone https://github.com/artyom12211/ibookly-client\n
pnpm i\n

добавь `.env.development` 
```
VITE_API_HOST=http://localhost:4000 #хост на котором работает бэк
VITE_BOT_NAME=                      #имя тг бота (задается при создании бота через @BotFather)
VITE_MINIAPP_NAME=                  #имя мини приложения (задается при создании мини апп через @BotFather) 
```
### Старт
```
pnpm dev:https
```

## Бэкенд:
[ibookly-backend](https://github.com/artyom12211/ibookly-server)\n
cd /backend\n
git clone https://github.com/artyom12211/ibookly-server\n
pnpm i\n

добавь `.env.development`
```
API_PREFIX=""
PORT=4000
TELEGRAM_BOT_TOKEN=<YOUR_BOT_TOKEN> #токен тг бота (получить можно через @BotFather)
USE_MOCK_DATA=true                  #поставь true, если хочешь сразу увидет результат, иначе нужно настроить бд
BOT_NAME=                           #имя тг бота (задается при создании бота через @BotFather)
APP_NAME=                           #имя мини приложения (задается при создании мини апп через @BotFather) 
```

### Старт
```
pnpm start:dev
```
