# Подсказка по Git

## Базовые команды:

Создания репозитория, команда:
```sh
git init
```
### Отслеживание файла до сохранения изменений

Для добавления изменений в коммит(отслеживания),команда:

```sh
git add <file name>
```
### Сохранение текущего состояния файла

Для добавления коммита(сохранения текущего состояния) используется команда:
```sh
git commit -m "Краткое описание сохраниения"
```
### Журнал коммитов

Для просмотра журнала коммитов 
 (отображения всех) , использовать команду:
```sh
git log
```

А, если вы хотите отобразить все **коммиты** в краткой записи ( название и краткий хэш),то воспользуйтесь командой:

```sh
git log --oneline
```

Для того, чтобы увидеть расположение коммитов в виде отображения их как диаграммы с ветками,нужно воспользоваться командой:

```sh
git log --oneline --graph
```
### Переключение между ветками и коммитами
 
Если вы хотите вернуться к предыдущему коммиту(сохранению) или перейти на другую ветку, то воспользуйтесть командой:

```sh
git checkout <имя 
 ветки/ краткий хеш коммита>
```
### Сравнение текущего состояния с последним сохранением

Если нужно сравнить *текущее* состояние файла по отношению к последнему сохранению(коммиту), то есть команда:
```sh
git diff
```

Для того, чтобы посмотреть состояние папки с репозиторием и наличие изменений в файлах, нужно воспользоватся командой:

```sh
git status
```
!Но, только обязательно проверить путь в терминале( чтобы вел к папке с репозиторием) !

## Управление ветками

Отображение всех веток, это команда:

```sh
git branch
```
### Создать новую ветку

Если необходимо создать новую ветку, то можно воспользоваться командой:

```sh
git branch <branch_name>
```
### Удаление ветки

Если вы хотите удалить ветку, то можно воспользоваться командой:

```sh
git branch -d <имя_ветки>
```
# Команды для работы с удаленными репозиториями

## Как склонировать внешний репозиторий на свой Пк
 Для того чтобы склонировать внешний(удаленный)репозиторий на свой пк, нам нужно вопользовваться командой:
 ```sh
 git clone <адрес репозитория>
 ```

 ## Как скачать все актуальные изменения с удаленного репозитория и автоматически сделать слияние с нашей версией

 Для этого нам понадобиться команда:

 ```sh
 git pull
 ```

 ## Отправить изменения в удаленный репозиторий с локального

 Команда позволяет отправить нашу текущую версию репозитория на внешний репозиторий. Требует авторизации на внешнем репозитории:
 
 ```sh
 git push
 ```