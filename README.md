# Домашнее задание к занятию "`Управление доступом`" - `Бакулев Евгений`

## Задание 1. Создайте конфигурацию для подключения пользователя

- [Манифест запроса](https://github.com/garrkiss/kuber-user/blob/main/manifest/certrequest.yaml)
- [Манифест Deployment ](https://github.com/garrkiss/kuber-config-app/blob/main/manifest/task1/configmap-env.yaml)
- [Манифест rbac](https://github.com/garrkiss/kuber-config-app/blob/main/manifest/task1/configmap-html.yaml)

Генерируем ключ и запрос на выпуск сертификата
![Ссылка](https://github.com/garrkiss/kuber-user/blob/main/img/1.png)

Применяем деплоймент с подами для теста и переключаем контекст, видим что запрос get po работает, без включенного rbac
![Ссылка](https://github.com/garrkiss/kuber-user/blob/main/img/2.png)

Включаем rbac и пробуем обратиться к поду и получаем ошибку. Применяем роль и привязку к пользователю
![Ссылка](https://github.com/garrkiss/kuber-user/blob/main/img/3.png)

Проверяем доступ к поду
![Ссылка](https://github.com/garrkiss/kuber-user/blob/main/img/4.png)


