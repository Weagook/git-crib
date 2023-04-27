# git-crib

## Первоначальная настройка

Ввести данные

	git config --global user.name "Noname Incognito"
	git config --global user.email innoname@email.com
	
Проверить настройки

	git config --list
	
Чтобы проверить конкретную информацию (допустим имя)

	git config user.name
	
Также git config позволяет изменить визуальный вывод данных для пользователя - настройки интерфейса могут облегчить восприятие, выделив нужные места разными цветами:

	git config --global color.ui true
	
Для создания нового проекта в GIT необходимо:

	git init
	
Для добавления файлов в Git необходимо добавить их в индекс и произвести коммит, используя команды git add и git commit:

	git add .
	git commit -m 'initial project version'

Для клонирования репозитория:

	git clone https://github.com/Weagook/weagook.git
	
Для проверки статуса файлов использовать команду:

	git status
	
Команда git diff отвечает на несколько вопросов, например, какие именно изменения не были проиндексированы (git diff) и какие именно проиндексированные изменения войдут в следующий коммит (git diff --staged или git diff --cached).

Для загрузки изменений необходимо добавить все необходимое командой

	git add .

Закомитить

	git commit -m "my commit"

И сделать пуш в репозиторий

	git push <remote-name> <branch-name>
