# **Инструкция по работе с системой контроля версий Git**
* Git - распределенная система управления версиями, созданная Линусом Торвальдсом.


## Инициализация репозитория

### Чтобы инициализировать новый репозиторий нужно ввести в терминале команду:
    git init

## Проверка состояния репозитория
### Чтобы контролировать текущее состояние нашего проекта в репозитории, нужно ввести в терминале команду:
    git status

## Добавление версионности
### Чтобы отслеживать изменения в файле, для последующей фиксации, необходимо ввести команду:
    git add (имя файла)

## Фиксация изменений
### Чтобы зафиксировать изменения в файле проекта, нужно ввести команду:
    git commit

### Чтобы не путаться в в изменениях, необходимо давать им названия командой:
    git commit -m ("имя коммита(фиксации")

 ## Просмотр истории создания коммитов
 ### Чтобы посмотреть ранее созданные коммиты, необходимо ввести команду:
    git log  

### Чтобы увидеть состояние лога (коммит в одну строку), необходимо ввести команду:
    git log --oneline

### Чтобы увидеть все коммиты в список, необходимо ввести команду:
    git log --all

## Переключение между версиями
### Чтобы переключиться на ранее сохраненную версию репозитория, необходимо ввести команду:
    git checkout(hash)

## Информация между различиями среди коммитов
### Для просмотра разницы между сохраненным файлом на диске и последним закоммиченным, используется команда:
    git diff

## Ветвления
В процессе работы над своим проектом мы сталкиваемся с необходимостью внесения правок, улучшений и даже некоторых удалений данных нашей работы. Крайне неудобно работать с множеством коммитов, с разными датами и похожими заголовками. Гораздо удобнее сделать, так называемое, *ветвление*. Ветвление позволяет нам создавать изменения,улучшения, правки и т.д., параллельно с основной работой над проектом. С последующим слиянием веток с основным деревом проекта и удалением их. 

    
## Создание новых веток
Для того чтобы создать новую ветку, необходимо в терминале ввести команду:

    git branch <name>
Где "name" означает имя нашей ветки. Далее, переходим на эту ветку, вносим нашу информацию и создаем коммит. Ветка, с необходимой нам информацией, готова!

## Слияние новых веток
Для того чтобы выполнить слияние веток, необходимо, **находясь в *главной* ветке (в нее мы будем вливать другую ветку)**, выполнить команду:

    git merge <имя влитой ветки>
Если не произойдет кофликт между ветками, значит данные одной ветки дополнят информацию в другой.
 
## Просмотр созданных веток
Для того чтобы увидеть существующие ветки нашего проекта, необходимо в терминале ввести команду:

    git branch
"Звездочкой" будет отмечена ветка, в которой мы находимся.

Для перемещения между ветками используем команду:
 
    git checkout name_branches

## Решения при конфликте
При слиянии веток возможен конфликт, когда одна и та же строка в различных версиях, пишется по-разному.

*Git* может автоматически сохранить изменения разных версий, но далее нам  вручную необходимо откорректировать данные. Далее необходимо создать коммит о решении нами проблемы.

*VScod* предлагает 3 варианта : оставить первое, сохранить второе или работать с обоими изменениями.

## Удаление ветки
Для того чтобы удалить ветку (после слияния или ненужную), необходимо в терминале ввести команду:

    git branch -d <имя ветки>
Для удаления любой ветки используется команда:

    git branch -D <имя ветки>

## Удаленные репозитории

Удаленные репозитории представляют собой версии нашего проекта, сохраненные где-то (в сети, интернете).





