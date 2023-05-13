# Дипломное задание 3: веб-приложение

Описать элементы, которые использовались в тестах, с помощью Page Object.
* Для Page Object создан отдельный пакет.
* Для каждой страницы создан отдельный класс с Page Object.
* Тесты разделены по функциональности. Для тестов созданы отдельные классы.
* Все элементы страниц, которые используеются в тестах, описаны в Page Object.
* Название класса Page Object отражает его содержимое.
* Тесты запускаются и не падают.
* Тест — прежде всего проверка, а не набор действий. Каждый тест что-то проверяет.
* Протестирован функциональность в Google Chrome и Яндекс.Браузере.
* Подключен Allure-отчёт.

# Тесты UI
Регистрация
Проверено:

* Успешную регистрацию.
* Ошибку для некорректного пароля. Минимальный пароль — шесть символов.

Вход
Проверено:

* вход по кнопке «Войти в аккаунт» на главной,
* вход через кнопку «Личный кабинет»,
* вход через кнопку в форме регистрации,
* вход через кнопку в форме восстановления пароля.

Переход в личный кабинет

* Переход по клику на «Личный кабинет».
* Переход из личного кабинета в конструктор
* Переход по клику на «Конструктор» и на логотип Stellar Burgers.

Выход из аккаунта

* Выход по кнопке «Выйти» в личном кабинете.

Раздел «Конструктор»
Проверено, что работают переходы к разделам:

* «Булки»,
* «Соусы»,
* «Начинки».

Запуск
* Google Chrome: mvn clean test -Dbrowser=chrome
* Yandex Browser: mvn clean test -Dbrowser=yandex
