# Описание
Сборка базируется на:
  - [fiber](https://docs.gofiber.io/) + [air](https://github.com/cosmtrek/air) (go 1.19.3)
  - [postgres 15.1](https://www.postgresql.org/)
  - [vue 3](https://vuejs.org/) + [tailwind](https://tailwindcss.com/) + [postCSS](https://postcss.org/)

### Начало работы
  1. `git clone https://github.com/srsad/discount-service.git`
  2. создать файл `.env` в корне проекта и скопировать в него данные из `example.env`
  3. `docker-compose buid`, *последующии запуски `docker-compose up -d`**
      - `docker-compose up` запустит сервис postrges (+pgadmin) и `gofiber` - бэк.
      - Для того чтоб попать в контейнер fiber `docker-compose run --service-ports gofiber bash`

### Работа на фронте
  Необходима nodejs версии `16.13.0` или выше. Рекуомендуется установить [nvm](https://github.com/coreybutler/nvm-windows) для безболезненной смены ноды.
  После установки: 
  1. перейти в каталок `frontend`
  2. npm i
  3. npm run dev


**TODO**
  - `+` добавить образы для go(fiber)
  - `+` nodejs(vue3)
      - `~` собрать базу для vue, проверить порты
  - `+` добавиьт описание к разворачиванию окружения (docker-compose buid || docker-compose up)
  - разобраться с pgadmin
  - 
  - ...

**Fiber**
  - добавить тестовый эндпоинт
  - настройки линтера
  - 
  - ...

**Vue**
  - `+` подключить TS
  - `+` настройки линтера
  - `+` выборать библиотеку компонентов
  - `+` проработать архитектуру проекта (учесть composition api + pinia (нужна/нет)) - нужна
  - `+` создать дэмо страницу/страницы
  - `+` подключить `tailwind`
  - 
  - ...
