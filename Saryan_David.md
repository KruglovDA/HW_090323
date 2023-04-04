Инструкция по использованию Git

1. Проверка настроек

 git --version

2. Настройка git

* git config global user.name - задать имя
* git config global user.email - задать email

3. Создание проекта

* mkdir test - создание папки test
* cd test - переходим внутрь папки тест
* git init - создание локального репозитория

4. Создание первого коммита

* git add ... - добавить файл под контроль git

* git commit -m "" - создание первого коммита с комментарием

5. Статус проекта

* git status

6. История проекта

* git log

7. Переключение веток/коммитов

* git checkout название ветки/коммита

8. Ветки

* git branch - выводит список веток (звездочкой (*) омечает ветку, на которой мы находимся)
* git branch branch_name - создание ветки под названием branch_name
* git checkout branch_name - переключение на ветку branch_name
* git checkout -b branch_name - создали и сразу переключились на ветку branch_name

8.1. Переименование веток

* git branch -m branch1 branch2 - переименовали ветку branch1 в branch2

8.2. Удаление ветки

* git branch -D to_delete - удаляем ветку to_delete

8.3. Слияние веток
в момент слияния мы должны находиться в ветке, куда будем сливать изменения

* git merge test - слиянение ветки test в *main

9. Удаленный репозиторий
* git remote add origin "адрес" - отправить свой проект на github
* git push github main - отправляет ветку на удаленный репозиторий (где github - псевдоним для полного адреса)
* git remote - список доступных удаленных репозиториев
* git clone - клонирование репозитория
* git pull origin main - скачать изменения с удаленного сервера с указанием ветки
* git push origin main - отправить ветку на сервер

Спасибо!