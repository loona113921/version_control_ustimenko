# Подсказка по Git

Создание репозитория:
```sh
git init
```

Добавление содержимого рабочего каталога:
```sh
git add
```

Фиксирует изменение и сообщает о появлении новых версий:
```sh
git commit -m "комментарий"
```
Выводит список всех commit в хронологическом порядке:
```sh
git log
```
Тоже выводит список коммитов, только в укороченном варианте:
```sh
git log --oneline
```
Позволяет переключаться между версиями:
```sh
git checkout
```
Показывает разницу между текущей версией и ранее зафиксированной:
```sh
gif diff
```

**Инструкция по работе с удаленными репозиториями**

1. Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку Fork на странице репозитория https://git@github.com:gulden-geekbrains/version_control.git

2. Выполняем команду клонирования из своей fork-копии
git clone git@github.com:*YOURE_GITHUB*/version_control.git

3.Создаем новую ветку и вносим необходимые изменения в файл
git checkout -b updatereadme
vim README.md
git add README.md
git commit -m "Добавили инструкцию как создать pull request"

Делаем push
git push --set-upstream origin updatereadme
Переходим на свою страницу репозитория. Выбираем ветку updatereadme и жмем кнопку Compare & pull request
