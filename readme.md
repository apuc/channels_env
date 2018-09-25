## Инструкция по установке

1. Склонировать репазиторий ветка мастер
2. Скопировать содержимое файла ```.env.example``` в ```.env```
3. Прописать свои локальные настройки в ```.env```
4. Запустить команду ```docker-compose up```
5. Создать БД в контейнере ```mysql```
   * ```docker-compose exec mysql /bin/bash``` - подключение к контейнеру
   * ```mysql -u root -p``` - подключение у mysql
   * ```CREATE DATABASE {database_name};```
6. Указать в файле ```/nginx/sites/channels.conf``` порт Nodejs из файла ```.env```


## Структура директорий

|   |   | 
|---:|---|
| ./channels   |   |
|--- | laravel_channels  | 
|---   |vue_channels   | 
|---| express_channels|
|---| environment|
