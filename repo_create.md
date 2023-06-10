[<к содержанию](./readme.md)

# Создание GIT-репозитория

Обычно вы получаете репозиторий GIT одним из двух способов:

1. Вы можете взять локальный каталог, который в настоящее время не находится под версионным контролем, и превратить его в репозиторий GIT, либо

2. Вы можете клонировать существующий репозиторий GIT из любого места.

В обоих случаях вы получите готовый к работе GIT-репозиторий на вашем компьютере.

## Создание репозитория в существующем каталоге
---

Обязательно перейдите в каталог проекта, который не находится под версионным контролем GIT, а затем выполните команду:

`$ git init`

Эта команда создаёт в текущем каталоге новый подкаталог с именем .git, содержащий все необходимые файлы репозитория — структуру GIT-репозитория.

Если вы хотите добавить под версионный контроль существующие файлы (в отличие от пустого каталога), вам стоит добавить их в индекс и осуществить первый коммит изменений. Добиться этого вы сможете запустив команду `git add` несколько раз, указав индексируемые файлы, а затем выполнив `git commit`:
```
$ git add *.c
$ git add LICENSE
$ git commit -m 'Initial project version'
```
Подрбнее смотри раздел ***III. Основные команды*** 

## Клонирование существующего репозитория
---

Клонирование репозитория осуществляется командой 

`git clone <url>`

 Например, если вы хотите клонировать библиотеку libgit2, вы можете сделать это следующим образом:

```
$ git clone https://github.com/libgit2/libgit2
```
Эта команда создаёт каталог libgit2, инициализирует в нём подкаталог .git, скачивает все данные для этого репозитория и извлекает рабочую копию последней версии. Если вы перейдёте в только что созданный каталог libgit2, то увидите в нём файлы проекта, готовые для работы или использования. Для того, чтобы клонировать репозиторий в каталог с именем, отличающимся от libgit2, необходимо указать желаемое имя, как параметр командной строки:
```
$ git clone https://github.com/libgit2/libgit2 mylibgit
```
Эта команда делает всё то же самое, что и предыдущая, только результирующий каталог будет назван mylibgit.

[prev](config.md) | [next](repo_change.md)