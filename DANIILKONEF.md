# Что такое Git и зачем он нужен?
Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

## Команды 1й лекции

1. Команда **git --version** -  позволяет убедиться что GIT у вас уже установлен и заодно узнать какая версия стоит; 
2. Команда **git config --global user.name "DANIIL KONEF"** - позволяет задать имя пользователя текущего репозитория в текущем аккаунте операционной системы, имя пишется в кавычках, для примера написано "DANIIL KONEF", вместо этого должно быть указано Ваше имя. 
- Первое, что вам следует сделать после установки Git — указать ваше имя и адрес электронной почты. Это важно, потому что каждый коммит в Git содержит эту информацию, и она включена в коммиты, передаваемые вами, и не может быть далее изменена. 
- Если указана опция **--global**, то эти настройки достаточно сделать только один раз, поскольку в этом случае Git будет использовать эти данные для всего, что вы делаете в этой системе. Если для каких-то отдельных проектов вы хотите указать другое имя или электронную почту, можно выполнить эту же команду без параметра --global в каталоге с нужным проектом.
3. Команда **git config --global user.email "DANIILKONEF@yandex.ru"** - позволяет задать емейл пользователя текущего репозитория в текущем аккаунте операционной системы,  пишется в кавычках, для примера написано "DANIILKONEF@yandex.ru", вместо этого должен быть указан Ваше емейл.
4. Команда **git config --list** - позволяет вывести на экран терминала все текущие настройки, сохраненные в Гите. *Эта команда не изучалась в лекциии и на семинаре*.
5. Команда **git init** - позволяет создать тот самый заветный репозиторий в текущей папке, в которой запущен сейчас консольный терминал. После создания репозитория, можно пользоваться командами дальше по списку.
6. Команда **git add .** - позволяет добавить в кэщ/стэш все файлы в папке репозитория для того чтобы их потом можно было закоммтить/сохранить. Точка после add отвечает за то чтобы Гит учел именно все файлы репозитория;
7. Команда **git add .** - позволяет добавить только одни файл в папке репозитория в в кэщ/стэш для того чтобы потом его можно было закоммтить/сохранить. Для этого после add нужно либо написать полное имя файла либо воспользоваться автоматизированным переборов всех файлов при помощи клаваши **Tab**.
8. Команда **git commit -m "Необязательный комментарий"** - позволяет сохранить/закоммитить все нужные файлы в текущем их состоянии, положив их в репозиторий. Должна выполнять после команды **add**, описанной ранее.
9. Команда **git branch name_of_branch** - создает ветку с именем name_of_branch;
10. Команда **git merge from_branch_name** - выполняет слияние ветки from_branch_name в текущую ветку;
11. Команда **git checkout to_branch_name** - выполняет переход с текущей ветки на ветку под именем to_branch_name;
12. Команда **git branch** - отображает все имеющиеся ветки в репохитории; // не получилось слить почему то, потерялась строка при решении конфликта, пробую еще раз.
13. Комнада **git reset** - выполняет отмену коммита;
14. Команда **git stash** - временно прячет в скрытый кэш изменения текущих файлов не готовых к коммиту;


## Полезные ссылки
- [ссылка1](https://gist.github.com/Jekins/2bf2d0638163f1294637/ "Статейка на ГитХабе о языке разметки Маркдаун")
- [ссылка2](https://learn.microsoft.com/ru-ru/contribute/markdown-reference/ "Справка от Майкрософт о языке разметки Маркдаун")
- [ссылка3](https://habr.com/ru/post/541258/ "Статья на ГитХабе Git для новичков (часть 1)")
- [ссылка4](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%9F%D0%B5%D1%80%D0%B2%D0%BE%D0%BD%D0%B0%D1%87%D0%B0%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F-%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-Git "1.6 Введение - Первоначальная настройка Git")