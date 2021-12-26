# Git и удаленный репозиторий
Что такое git
Гит - это система контроля версий, которая помогает отслеживать историю изменений в файлах. Git используют программисты для совместной работы над проектами.

## Создание локального репозитория
Создать локальный репозиторий можно с помощью команды *git init*. Для этого надо применить эту команду в той папке, где в будущем будет репозиторий.

## Добавление файлов в репозиторий
Версионность к файлу добавляется с помощью команды *git add*. Команда применяется следующим образом *git add <название файла>*

## Создание коммита
Для того, чтобы создать новый коммит необходимо использовать команду *git commit*. Применяется она следующим образом: *git commit -m "<сообщение к коммиту>"*. Сообщения к коммиту писать ***ОБЯЗАТЕЛЬНО***!

## Просмотр наличия изменений
Для того, чтобы посмотреть имеются ли изменения в локальном репозитории используется команда *git status*. Достаточно её просто применить в папке с препозиторием

## Просмотр разницы между текущей версией и последней "сохранённой"

Для того, чтобы посмотреть разницу между последним коммитом и текущей версией файлов, используется команда *git diff*. Достаточно её просто применить в папке с репозиторием

## Просмотр истории коммитов

Для просмотра истории коммитов используется команда *git log*. Для того, чтобы увидеть историю коммитов, достаточно просто применить эту команду в папке с репозиторием.

## Перемещения между изменениями

Для того, чтобы переместиться на какое-то из прошлых изменений необходимо использовать команду *git checkout*. Применяется она следующим образом в папке с репозиторием: *git checkout <номер коммита>*. Для возврата к последнему коммиту ветки нужно использовать команду *git checkout master*

## Работа с ветками


### Просмотр списка веток

Для того, чтобы просмотреть список имеющихся веток, необходимо использовать команду *git branch*. Для этого в папке с репозиторием пишем команду *git branch*.

### Создание новой ветки

Для того, чтобы создать новую ветку, необходимо использовать команду *git branch*. Используется она в папке с репозиторием следующим образом: *git branch <название новой ветки>* 

## Слияние веток

Для слияния веток используется команда *git merge*. Приняется она в папке с репозиторием следующим образом: *git merge <название ветки>*. В процессе слияния может произойти ***КОНФЛИКТ*** или слияние может произойти автоматически

## Git clone
Для копирования чужого репозитория в свой используем команду git clone 

Подготовка репозитория
Обычно вы получаете репозиторий Git одним из двух способов:

Вы можете взять локальный каталог, который в настоящее время не находится под версионным контролем, и превратить его в репозиторий Git, либо

Вы можете клонировать существующий репозиторий Git из любого места.

В обоих случаях вы получите готовый к работе Git репозиторий на вашем компьютере.

Создание репозитория в существующем каталоге Если у вас уже есть проект в каталоге, который не находится под версионным контролем Git, то для начала нужно перейти в него. Если вы не делали этого раньше, то для разных операционных систем это выглядит по-разному:

а затем выполните команду: для Windows:

$ cd C:/Users/user/my_project



$ git init
Создание сохранений
тут и add, и status, и commit? тут и add, и status, и commit!

Перемещение между сохранениями
Для переключения между "сохранениями"(коммитами), необходимо использовать команду git checkout следующим образом: git checkout <номер коммита для переключения>. Номер коммита берётся из истории коммитов и на него произойдёт переключение.

Журнал изменений (git log)
Журнал изменений — это файл, который содержит общий, хронологически упорядоченный список изменений, внесенных в проект. Он часто организован по версии с указанием даты, после чего следует список добавленных, переработанных и удаленных функций.

В общем смысле, существует два способа делать записи в журнал изменений.

Обычный способ: Cоздайте текстовый файл и начните перечислять все внесенные вами изменения с указанием определенной даты.
Выбор разработчика (он же вариант для ленивых): автоматическое создание списка изменений из ваших сообщений к коммитам.
Журнал изменений представляет собой программное протоколирование изменений, вносимых в большой проект. Таким проектом может быть веб-сайт или проект программного обеспечения. Обычно записи журнала изменений содержат информацию об исправлении ошибок, о новых возможностях и т.д.

Ветки в git
Ветка представляет собой отдельное направление разработки. Ветки выступают в качестве абстрактного представления для процесса редактирования/индексации/коммита. Можно рассматривать их как способ запросить новый рабочий каталог, раздел проиндексированных файлов и историю проекта. Новые коммиты записываются в историю текущей ветки, что приводит к образованию развилки в истории проекта.

Команда git branch позволяет создавать, просматривать, переименовывать и удалять ветки. Она не дает возможности переключаться между ветками или выполнять слияние разветвленной истории. Именно поэтому команда git branch тесно связана с командами git checkout и git merge.

Удаление веток
Чтобы удалить локальную ветку в Git нужно выполнить команду (вместо mybranch необходимо поставить название ветки, которую вы хотите удалить): git branch -d mybranch.

Обратите внимание на то, что ветка, которую вы удаляете, не должна быть вашей текущей веткой, в которой вы работаете, иначе отобразится ошибка

Работа с ветками
Просмотр списка веток
Для просмотра необходимо испоьзовать команду "git branch". Для этого в папке с репозиторием пишем эту команду

Создание новой ветки
Чтобы создать новую ветку необходимо использовать в папке репозитория команду "git branch название новой ветки"

Слияние веток
Для слияния веток используется команда "git merge название ветки" в папке репозитория. В процессе слияния может произойти *** конфликт *** или слияние может произойти автоматически
