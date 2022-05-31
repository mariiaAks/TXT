# TXT
GIT Homework 1

Все шаги сценария выполняйте в терминале GitBush, Terminal, в папке под гитом.

 1. Создать внешний репозиторий c названием TXT.
 
        В веб интерфейсе github: create new repository TXT --public
  2. Клонировать репозиторий TXT на локальный компьютер.
 
         $ git clone git@github.com:mariiaAks/TXT.git
 
 3. Внутри локального TXT создать файл “new.txt”.
 
        $ cd TXT
        $ touch new.txt
 4. Добавить файл под гит.
 
        $ git add new.txt
 
 5. Закоммитить файл.
 
        $ git commit -m "Add new file new.txt"
  
 6. Отправить файл на внешний GitHub репозиторий.
 
        $ git push 
 
 7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.
 
        $ vim new.txt
        INSERT (кнопка i)
 
        ФИО - Щербатова Мария Романовна
        Возраст - 38 лет
        Количество домашних животных - 0
        Желаемая зарплата - 100000 руб.

        Esc :wq
 8. Отправить изменения на внешний репозиторий.
 
        $ git add new.txt
        $ git commit -m "Change file new.txt: add personalInfo"
        $ git push
 
 9. Создать файл preferences.txt
 
        $ touch preferences.txt
  
 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT.
 
    $ vim preferences.txt
    INSERT (кнопка i)
	  Предпочтения:
	  Любимый фильм - "Летят журавли"
	  Любимый сериал - "Склифосовский"
	  Любимая еда - Тортики
	  Любомое время года - Лето
	  Страна, которую хотела бы посетить - Дания

    Esc :wq 
  11. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT
  
    $ cat > sklls.txt
    Скиллы, которые будут изучены на курсе:
	1. Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования
	2. Клиент-серверная архитектура, структура http запросов и ответов
	3. Тестирование API через Postman
	4. Тестирование веб-приложений, DevTools браузеров, снифинг web трафика через Charles и Fiddler
	5. Тестирование мобильных приложений, Android studio, перехват мобильного через Charles и Fiddler
	6. Установка и настройка БД Postgres, основы SQL"
 
    Ctrl+C
 
 12. Сделать коммит в одну строку.
 
    $ git add preferences.txt sklls.txt && git commit -m "Add 2 files preferences.txt sklls.txt"
  
 13. Отправить сразу 2 файла на внешний репозиторий.

    $ git push 
  
 14. На веб интерфейсе создать файл bug_report.txt.
 
    Add file - Create new file - Commit new file
 
 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
    Commit changes
 
 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT.
  
    Bug_id: 1
    Title: Dash line not visible on widget
    Severity: major
    Priority: high
    Summary: 
    Precondition: Clear screen
    StepToReproduce: 
	1) Add several widgets
	2) Change size some widgets
    Environment: 
    1) Redmi Note 7 MIUI 12.5.1.0 android 10 QKQ1.190910.002
	2) Honor 20 pro (YAL-L41), Android 10
    ExpectedResult: Widgets have a dotted line on all 4 sides
    ActualResult: Widgets don't have dotted lines
    Attachments: 
 
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
    Commit changes
  
 18. Синхронизировать внешний и локальный репозиторий TXT
 
    $ git pull
