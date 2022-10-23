# PhonebookBot

Создать телефонный справочник с возможностью импорта и экспорта данных в нескольких форматах.
- под форматами понимаем структуру файлов, например: в файле на одной строке хранится одна часть записи, разделитель - пустая строка:

Фамилия_1  
Имя_1  
Телефон_1    
Описание_1  
Фамилия_2    

Имя_2    
Телефон_2    
Описание_2    
и т.д.

в файле на одной строке хранится все записи, символ разделитель - ",":
Фамилия_1,Имя_1,Телефон_1,Описание_1
Фамилия_2,Имя_2,Телефон_2,Описание_2
и т.д.

# Как запустить проект (рекомендуем использовать VCS)

# Для запуска с помощью консоли:
1. Cкачать проект в локальный репозиторий;
2. B консоли ввести команду "python3 main.py";
3. B случае необходимости создания рандомной базы контактов раскоменнтировать строку #7 (метод dg.start()) модуля main.py;
4. Cледовать инструкциям в консоле.
# Для запуска телеграм-бота:
1. Cкачать проект в локальный репозиторий;
2. обновить Python до версии 3.10.5;
3. настроить окружение, введя в консоле поочередно команды:

python3 -m venv .libraries

pip install pyTelegramBotAPI

4. При необходимости обновить библиотеку до последней версии (следуя инструкциям в консоле)
5. Перезапустить консоль;
6. B корневой папке проекта (phonebook) создать файл с названием "token.csv", в котором в первой строке добавить индивидуальный токен телеграм-бота, после чего сохранить изменения файла;
7. Инструкция по созданию индивидуального токена телеграм-бота здесь: https://core.telegram.org/bots
8. В консоле ввести команду "python3 bot.py" или "python bot.py" (при необходимости установить версию Python 3.10.5)