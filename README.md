Создай пустой проект

## Общее
`npm i -G pnpm`

## Фронтенд:
[фронт репа](https://github.com/artyom12211/ibookly-client)  
```
git clone https://github.com/artyom12211/ibookly-client  
cd .\ibookly-client\
pnpm i  
```

добавь `.env.development` 
```
VITE_API_HOST=http://localhost:4000 #хост на котором работает бэк
VITE_BOT_NAME=                      #имя тг бота, к примеру helloBot (задается при создании бота через @BotFather)
VITE_MINIAPP_NAME=                  #имя мини приложения, к примеру app (задается при создании мини апп через @BotFather) 
```
### Старт
```
pnpm dev:https
```
После запуска vite выдаст ссылку на проект: 
К примеру ➜  **Network: https://192.168.2.90:5173/ibookly** 
Установите эту ссылку для вашего мини приложения в тг.  

## Бэкенд:
[бэк репа](https://github.com/artyom12211/ibookly-server)  
```
git clone https://github.com/artyom12211/ibookly-server
cd .\ibookly-server\
pnpm i
pnpm dlx prisma generate
```

добавь `.env.development`
```
API_PREFIX=""
PORT=4000
TELEGRAM_BOT_TOKEN=<YOUR_BOT_TOKEN> #токен тг бота (получить можно через @BotFather)
USE_MOCK_DATA=true                  #поставь true, если хочешь сразу увидет результат, иначе нужно настроить бд
BOT_NAME=                           #имя тг бота, к примеру helloBot (задается при создании бота через @BotFather)
APP_NAME=                           #имя мини приложения, к примеру app (задается при создании мини апп через @BotFather) 
```

### Старт
```
pnpm start:dev
```
