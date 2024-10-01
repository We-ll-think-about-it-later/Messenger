## Запуск

Клонируем репозиторий с подмодулями
```sh
git clone --recurse-submodules https://github.com/We-ll-think-about-it-later/identity-service.git
```

Переименовываем файл шаблона окружения в .env
```sh
mv env.template .env
```

Запускаем Docker-контейнеры
```sh
docker-compose up -d --build
```

## Backend

### Аутентификация
Для всех эндпоинтов, кроме `/auth/*`, требуется access токен:
```
Authorization: Bearer <access токен>
```

### Разделы API

- [Авторизация и профиль](https://github.com/We-ll-think-about-it-later/identity-service?tab=readme-ov-file#%D1%80%D1%83%D1%87%D0%BA%D0%B8)
