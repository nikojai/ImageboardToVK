# Imagebord to VK

Имиджбо́рд (англ. imageboard — «доска изображений») имеет достаточно большую популярность в РУ-сегменте. Для портирования изображений из имиджборд сервисов в социальную сеть "VK" с минимальной рутиной можно использовать это решение.

## Dependencies

  1. [nlohmann_json](https://github.com/nlohmann/json)
    Обработка JSON ответов от имиджборда и манипуляции с ними.
  2. [cpr](https://github.com/libcpr/cpr)
    CURL wrapper, post/get запросы с серверу
  3. [httplib](https://github.com/yhirose/cpp-httplib)
    Возможность создать свой локальный сервер с методами для управления приложением.
  4. [inja](https://github.com/pantor/inja)
    Возможность строить html страницы для юзер экспириенса на лету

## How to use

1. В CMake файле проекта не предусмотрен FetchContent зависимостей, поэтому необходимо иметь установленные библиотеки уже на своём ПК. Подробнее об этом можно узнать в репозиториях библиотек.
2. Проект проверенно работает с компилятором GCC 13.2.0. Скомпилируйте и откройте бинарный файл.
3. Откройте любой браузер и перейдите по ссылке http://localhost:8080/
4. Выберите контент который необходимо увидеть в сообществе.
5. Нажмите на кнопку "Отправить"