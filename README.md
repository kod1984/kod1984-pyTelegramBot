# kod1984-pyTelegramBot
1st bot

#Пример максимально простого бота для Телеграм. Для рассылки новостей в группы телеграм куда его добавили и проёма заявок от заинтересовавшихся пользователей.
Работает без БД. Все данные хранит в файлах который сам же и создаёт при первом запуске.
Необходимые файлы для работы:
cb.py
config_reader.py
.env

В файле .env нужно прописать токен своего бота. Бот создаётся через Телеграм путем запроса у @BotFather.
в .env одна строка:
BOT_TOKEN = 98999999:SDgfkdslkfdsltrWWE12

!ВАЖНО! Бот не знает в какие группы он уже добавлен. Он узнаёт это только в момент добавления и сохраняет в файл. 
Соответственно скрипт должен быть запущен в момент добавления в группу.
Админа, по умолчанию нет. Что запросить роль админа, отправь боту команду "/godmoe 123". 123 можешь поменять на что хочешь. 
После этого ID телеграм акаунта запросившего роль админа появится в файле "adminsNewID.txt". Туда будут попадать ID всех кто эту команду боту отправит. 
ID того нужно сделать админом переместить в файл "adminsID.txt"