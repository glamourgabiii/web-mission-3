# Mission 2

## Part 0

[Link to video](https://www.youtube.com/watch?v=UUhavvMO2FQ)

## Part1

- Вопрос 1	 
SSH — это защищённый способ подключаться к удалённым серверам и управлять ими через терминал. Он шифрует соединение, поэтому команды и передаваемые данные остаются в безопасности и защищены от перехватов.

- Вопрос 2	 
Публичный SSH-ключ Васи заносим в файл:
~/.ssh/authorized_keys
(Сначала открываем его через nano, вносим туда ключ, сохраняем, и проверяем права через chmod 600 ~/.ssh/authorized_keys)

- Вопрос 3	 
Long Polling — клиент в данном случае самостоятельно запрашивает апдейты. Если данных нет, сервер ждёт, а потом либо отвечает с данными, либо говорит: "Ничего нового". Затем сразу делается новый запрос. Полинг при этом нагружает сервер, потому что он получает много запросов. Webhooks — это обновления в реальном времени, сервер сам отправляет данные клиенту, как только они появляются. Клиент просто ожидает входящих сообщений, не дёргая сервер.

- Вопрос 4	 
Компании и проекты выкладывают свой код и публично сообщают о багах и проблемах в коде, и выкладывают это в раздел issues. Любой желающий может откликнуться, оставив коммент и попытаться решить проблему/взяться за разработку новой фичи? Для этого они делают форк репозитория, вносят правки и делают пул реквест, после чего команда проекта может принять изменения и код любого желающего может стать частью проекта.
Здесь нашла issues своей прошлой компани:
https://github.com/pontem-network/coins-registry/issues/58
А здесь для Blum:
https://github.com/petyasoft/Blum/issues/61

- Вопрос 5	 
Добавить файл заглушку .gitkeep (например) в папку
Дальше добавляем этот файл в репозиторий и не забываем закомитить 
