# Руководство пользователя 
## Инициализация 

* *git init* - команда, которая из обычной папки создает репозиторий; 

* *git clone* - загружает внешний репозиторий на наш ПК. 

## Локальные команды 

* *git add* - добавляет файл в репозиторий; 

* *git status* - показывает текущее состояние, есть ли изменения, которые нужно запомнить (сохранить); 

* *git diff* - показывает разницу между текущим файлом и сохраненным; 

* *git commit* - сохраняет изменения в репозиторий; 

* *git log* - журнал изменений;

* *git push* - позволяет отправить свою версию репозитория во внешний репозиторий;

* *git pull* - позволяет скачать всё из текущего репозитория и автоматически сделать *merge* с нашей версией.

## Ветвление и слияние 

* *git branch branch_name* - создание ветки; 

* *git checkout branch_name* - команда, которая позволяет переключаться с одной ветки на другую; 

* *git merge branch_name* - команда слияние веток; 

* *git branch -d branch_name* - удаление ветки 