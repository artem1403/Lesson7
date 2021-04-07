# Тренировка docker-compose

Поднять 2 сервиса, сборочный и продовый.
В сборочном сервисе должна происходить сборка Java приложения. В продовом - запуск приложения. Продовый образ должен быть минимальным по размеру.

# TODO
* [x] Вытащить boxfuse как папку submodule. Ссылка https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
* [ ] Добить мавен, чтобы поднимался контейнер, без сборки
* [ ] Сделать в мавене volume чтобы контейнер мог собирать приложения из него
* [ ] Собрать продовский контейнер с легковесным томкатом

## Памятка по командам
### Git submodules
Добавление подмодуля
```bash
git submodule add https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
```
При клонировании проекта с подмодулем делаем следующее
```bash
git submodule init
git submodule update
```