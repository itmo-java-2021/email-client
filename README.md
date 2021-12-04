# Учебный проект "Почтовый клиент"

## Структура

Проект поделен на Maven и Java модули
- client
- server
- model
- communication

### client

Содержит в себе простенький пользовательский интерфейс. Запускать обязательно необходимо указав свой имейл и хост сервера.
Например:
`fred@192.168.0.1`
Для программы нужно указать в качестве аргумента `--email=fred@192.168.0.1`.
Если нет возможности подключиться к серверу через ближайший роутер, то можете использовать программу ngrok: https://ngrok.com

В этом модуле необходимо сделать свою реализацию EmailClient.

## server

Содержит в себе реализацию TCP сервера. Должен запускаться на определённом порту и исполнять команды клиента.

## model

Содержит POJO классы, используемые как клиентом, так и сервером.

## communication

Содержит в себе классы команд и ответов для общения клиента и сервера. 

## Задачи:

1. Разработать протокол сетевого общения между клиентом и сервером и разместить его в модуле communication.
2. Научить сервер сохранять письма при перезапуске.
3. Добавить возможность удаления писем.
4. Добавить возможность отправлять письма нескольким получателям сразу.
5. Добавить логгер.