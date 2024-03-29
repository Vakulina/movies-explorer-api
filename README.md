## Бэкенд-часть сервиса Movies - сервиса по поиску и сохранению понравившихся фильмов с регистрацией и авторизацией (простой аналог "Кинопоиска")

```
ЛОГИН
test@test.su
ПАРОЛЬ
Test2023
```

#### [Деплой фронтенда](https://movies-onkf.onrender.com/)

![movies](https://github.com/Vakulina/movies-explorer-api/assets/80524794/da273458-e7ef-40c2-8514-37a8f4f6ad2b)

#### Функционал API:
| **Action**            | **method** | **URI** |
| --- | --- | --- |
| возвращает информацию о пользователе (email и имя) | GET | /users/me |
| обновляет информацию о пользователе | PATCH   | /users/me |
| возвращает  все сохранённые пользователем фильмы | GET  | /movies |
| создаёт фильм с переданными в теле данными | POST        | /movies |
| удаляет сохранённый фильм по _id | DELETE       | /movies/_id |
| создаёт пользователя с переданными в теле данными | POST        | /signup |
| возвращает и записывает в cookies присвоенный JWT, если в теле запроса переданы правильные почта и пароль | POST        | /signin |
| удаляет JWT из cookies | POST        | /signout |

### Используемые технологии:
- Express + MongoDB
- сервер nginx для деплоя на виртуальной машине

###  Для запуска на локальной машине:
- запустить сервер СУБД MongoDB (СУБД должна быть предварительно установлена)
- скачать содержимое ветки level-1
- установить зависимости командой **npm install**, запустить локальный сервер командой **npm run start** (на порту 3000)

### Планы по улучшению проекта
- типизация
- монорепозиторий для фронтенд и бэкенд части
- настроить переменные окружения

#### :link: Домен сервера (бэкенд) - https://759c6cd12fb9.vps.myjino.ru/users/me
#### :link: Деплой фронтенда - https://movies-onkf.onrender.com
#### :link: GitHub репозиторий (фронтенд) - https://github.com/Vakulina/movies-explorer-frontend


