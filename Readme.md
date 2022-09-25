# Инструкция по работе с Git

## Подготовка репозитория
Для создания репозитория используется команда *git init*. Чтобы созадать репозиторий напишите в терминале с открытой папкой для репозитория *git init*.

## Добавление файлов в репозиторий

Для добавления файла к коммиту используется комманда *git add*. Для этого в терминале с папкой-репозиторием необходимо написать *git add <название файла>*.

## Создание коммита
Для создания коммита используется команда *git commit*. Чтобы создать новый коммит в терминале с открытой папкой-репозиторием пишем команду *git commit -m "<сообщение к коммиту>"*. Сообщения к коммитам писать ***ОБЯЗАТЕЛЬНО***.

## Отчёт о состоянии
Для того, чтобы получить отчёт о состоянии   используется команда *git status*
После применения этой команды мы получаем список отредактированных файлов.
Если нам нужно получить не только список файлов, но и конкретную информацию -  какие строки добавлялись, какие удалялись, какие изменения были внесены - используется команда *git diff*

## Просмотр истории версий
Чтобы просмотреть  истроию изменений  используется команда *git log*.
Команда выводит в обратном хронологическом порядке список всех сохраненных в репозиторий версий. Самым первыми будут показаны самые последние коммиты.

## Ветвление
Команда *git branch* выодит на монитор список всех существующих веток. По умолчанию основная ветка называется *master*. 
Для добавления/создания ветки используется команда *git branch <название ветки>*
Чтобы перейти на новую ветку используем команду *git checkout <название ветки>*
Чтобы слить ветки используем команду *git merge*.
Для слияния веток сначала переходим  с помощью комнды *git checkout <название ветки>* в ту ветку, в основную, в которую будем добавлять.
Затем находясь в основной ветке командой *git merge <название ветки которую добавляем>* добавляем ветку. 

## Удаление ветки
Ветку, в которой отпала необходимость можно удалить. Для этого используем команду *git branch -d <название ветки>.

d от delete.

Лучше на начальном этапе освоения git использовать маленькую d, в таком случае  ветка будет удалена только после того как данные из этой ветки будут добавлены в основную.

## Графическое отображение веток
Чтобы получить графическое отображение используется команда git log --graph
