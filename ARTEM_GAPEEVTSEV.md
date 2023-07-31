
# Git. Руководство пользователя
## Основные команды

### Работа с репозиторием
* git init - инициализирует локальный коммит
* git add <путь> - добавление файлов/каталогов в index(область подготовленных файлов для последующей фиксации)
-m - сообщение коммита
* git push - добавить зафиксированные изменения в удаленный репозиторий
* git status - статус изменений в репозитории
* git log - показать хронологию коммитов

### Работа с коммитами
* git commit <параметры> - создает коммит\
-a - git add .( . - это путь того места где сейчас находимся)\
* git rebase - эта команда работает как с ветками так и с коммитами. Звучитк как перебазирование. С помощью нее например можно склеить(squashing) коммиты.\
git rebase -i HEAD~3 - выведеит 3 последние коммита. У каждого в начале будет команда pick. Если у первого оставим pick, у 2 и 3 заменим на squash, далее сохраним, то 3 коммита склеятся в один. Перед сохранением git даст выбрать имя коммита.

asasa
asasas
Какой то контен для ветки test2

### Работа с ветками
* git branch <параметры> <имя ветки> - создрать новую ветку\
-D - удалить ветку
* git checkout <параметры> <имя ветки> - переключиться на ветку или коммито\
-b - создать и переключиться на ветку
* git stash - спрятать текущие изменения. Полезно если например еще не готов коммит, но нужно переключиться на другую ветку. Для этого можно припрятать изменения и потом их опять извлечь.