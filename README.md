﻿# Это репозиторий для обучения pull request

## Первые шаги

1. Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку Fork на странице репозитория <https://git@github.com:gulden-geekbrains/version_control.git>
2. Выполняем команду клонирования из своей fork-копии
```sh
git clone git@github.com:*YOURE_GITHUB*/version_control.git
```
3. Создаем новую ветку и вносим необходимые изменения в файл
```sh
git checkout -b updatereadme
vim README.md
git add README.md
git commit -m "Добавили инструкцию как создать pull request"
```
4. Делаем push  
```sh
git push --set-upstream origin updatereadme
```
5. Переходим на свою страницу репозитория. Выбираем ветку **updatereadme** и жмем кнопку **Compare & pull request**

## Заметки

Что бы сделать push от другого пользователя необходимо выполнить команду
```sh
GIT_SSH_COMMAND='ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes' git push git@github.com:gulden-geekbrains/version_control.git
```

вместо *user-private-key* подставьте свой ключ

Можно прописать настройки для подсоединения по ssh
```sh
git config remote.origin.url git@github.com:gitusername/reponame
git config core.sshCommand "ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes"
```
# Как подружить git с github под Windows 10

Вот видео инструкция https://youtu.be/E8cIjbJMEpE

# Разграничение понятий Git и GitHub
 ### * Освоить работу с удаленными репозиториями, которые находятся не на локальной, а на удаленной машине, например, на сервере.
### * git — одна из систем контроля версий
### *Способ организации и поддержания версионности
### * Самая популярная система контроля версий

#
### * Сервис компании Майкрософт для организации работы удаленных репозиториев
### * Самый популярный сервис Git
### * Много полезных функций
### * Огромный архив различного кода
#

# Работа с удаленными репозиториями. Скачивание из текущего репозитория и слияние со своей версией.

### * Освоить работу с удаленными репозиториями, которые находятся не на локальной, а на удаленной машине, например, на сервере. Копировать внешний репозиторий на свой ПК можно командой git clone.

### * Команда git clone составная: она не только загружает все изменения, но и пытается слить все ветки на локальном компьютере и в удаленном репозитории.

### * git push - Отправить свою версию репозитория во внешний репозиторий поможет команда git push. При первом её использовании нужна git pull авторизация.

### * git pull - Эта команда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией
#
# Как настроить совместную работу

### Углубляемся в контроль версий

1. Создать аккаунт на GitHub.com
2. Создать локальный репозиторий
3. “Подружить” ваш локальный и удалённый репозитории. 
4. Отправить (push) ваш локальный репозиторий в удалённый (на GitHub), при этом, возможно, 
вам нужно будет авторизоваться на удалённом репозитории
5. Провести изменения “с другого компьютера”
6. Выкачать (pull) актуальное состояние из удалённого репозитория.
#
# pull request
### Углубляемся в контроль версий
#### ➜ команда для предложения изменений
#### ➜ запрос на вливание изменений в репозиторий
В больших компаниях один ответственный за проект создает аккаунт. Другие пользователи дают
команду pull request. Предлагать изменения на GitHub нужно в отдельной ветке. Сначала
пользователь копирует репозиторий на свой компьютер, делает fork репозитория, затем
клонирует версию на своём ПК, создаёт ветку с предлагаемыми изменениями, отправляет
изменения командой push в свой аккаунт на GitHub и даёт команду pull request.
# 
# Как сделать pull request
* Делаем   (ответвление) репозитория fork
* Делаем git clone   версии репозитория СВОЕЙ
* Создаем новую ветку и в НЕЕ вносим свои изменения
* Фиксируем изменения (делаем коммиты)
* Отправляем свою версию в свой GitHub
* На сайте GitHub нажимаем кнопку pull request

ссылка на репазиторий домащнего задания https://github.com/crazyCat56/-3.git



