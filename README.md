# salute-demo-app

##### Это небольшое Todo приложение (добавление, выполнение и удаление задач. [См. видео](https://youtu.be/P-o2rwHhARo)) может служить примером для работы с [Assistant Client](https://github.com/sberdevices/assistant-client). Для работы необходимо создать проект в "SmartApp Code" и смартап в "SmartApp Studio", сгенерировать token и запустить проект.

## Создание проекта в "SmartApp Code":

1. Идём на страницу SmartApp Code ([ссылка](https://smartapp-code.sberdevices.ru/));
1. Нажимаем "Создать проект";
1. Указываем "Имя";
1. Нажимаем "Создать";
1. Переходим на страницу с проектами ([ссылка](https://smartapp-code.sberdevices.ru/));
1. В меню проекта (кнопка "⋮") выбираем "Загрузить";
1. Выбирает архив "scenario-example.zip";
1. Нажимаем "Сценарии";
1. Нажимаем "Собрать";
1. Нажимаем "Публикации";
1. Нажимаем "Получить вебхук" (URL на Webhook в буфере обмена).

## Создание смартапа в "SmartApp Studio":

1. Идём на страницу SmartApp Studio ([ссылка](https://smartapp-studio.sberdevices.ru/));
1. Нажимаем "Создать смартап";
1. Указываем "Название смартапа" (указываем это же название в файле ".env.sample", в строке "REACT_APP_SMARTAPP");
1. Переключаем "Выбор типа смартапа" на "Canvas App";
1. Переключаем "Выбор инструмента" на "Есть готовое приложение";
1. Указываем URL на "Webhook";
1. Указываем URL на "Frontend Endpoint";
1. Нажимаем "Создать смартап".

## Генерация token:

1. Идём на страницу SmartApp Studio ([ссылка](https://smartapp-studio.sberdevices.ru/));
1. В меню пользователя (правый верхний угол) выбираем "Настройки профиля";
1. Нажимаем "Auth Token";
1. Нажимаем "Обновить ключ";
1. Нажимаем "Скопировать ключ" (сейчас token в буфере);
1. Указываем токен в файле ".env.sample", в строке "REACT_APP_TOKEN".
1. Переименовываем файл ".env.sample" в ".env".

## Запуск проекта:

```bash
npm install

npm run start
```
