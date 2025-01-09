# Sequence diagram

@startuml

actor Ребёнок as Child
participant "Интерфейс приложения" as UI
participant "Сервер" as Server
participant "База данных" as Database

Child -> UI: Открыть задание
UI -> Server: Запрос задания
Server -> Database: Получить данные задания
Database --> Server: Возвращает данные задания
Server --> UI: Передаёт данные задания
UI -> Child: Отображает задание и голосовую инструкцию

Child -> UI: Выбирает картинку
UI -> Server: Отправить выбор ребёнка
Server -> Database: Сравнить выбор с правильным ответом
Database --> Server: Возвращает результат проверки
Server --> UI: Передаёт результат проверки
UI -> Child: Отображает обратную связь (правильно/неправильно)

alt Правильный ответ
    UI -> Child: Показать анимацию успеха и похвалу
else Неправильный ответ
    UI -> Child: Показать правильный ответ
end

Child -> UI: Переход к следующему заданию
UI -> Server: Запрос нового задания
Server -> Database: Получить данные следующего задания
Database --> Server: Возвращает данные задания
Server --> UI: Передаёт данные задания
UI -> Child: Отображает новое задание

@enduml
