# План автоматизации тестирования возможности записи на обучение профессии "Тестировщик ПО" на сайте Netology.ru

## Перечень автоматизируемых сценариев
### 1) Переход на страницу профессии с главной страницы.
#### **1. Переход на страницу профессии через "Directions №1"**
##### Открыть страницу netology.ru.
##### Нажать на блок "Программирование".
##### Нажать на блок "Тестировщик ПО".
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **2. Переход на страницу профессии через "Directions №2"**
##### Открыть страницу netology.ru.
##### Нажать на блок "355 курсов всех направлений".
##### Нажать на блок "Тестировщик ПО".
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **3. Переход на страницу профессии через "Header №1"**
##### Открыть страницу netology.ru.
##### Нажать на блок "Каталог курсов".
##### В Навигаторе выбрать "Программирование".
##### Нажать на блок "Тестировщик ПО".
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **4. Переход на страницу профессии через "Header №2"**
##### Открыть страницу netology.ru.
##### Нажать на блок "Каталог курсов".
##### В Навигаторе выбрать "Полный каталог".
##### Нажать на блок "Тестировщик ПО".
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **5. Переход на страницу профессии через "Steps"**
##### Открыть страницу netology.ru.
##### Нажать на блок "Выбрать курс"
##### Нажать на блок "Тестировщик ПО"
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **6. Переход на страницу профессии через "Footer" №1**
##### Открыть страницу netology.ru.
##### Нажать на блок "Каталог курсов" в самом низу страницы
##### Нажать на блок "Тестировщик ПО"
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **7. Переход на страницу профессии через "Footer" №2**
##### Открыть страницу netology.ru.
##### Нажать на блок "Программирование" в самом низу страницы
##### Нажать на блок "Тестировщик ПО"
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
#### **8. Переход на страницу профессии через "Footer" №3**
##### Открыть страницу netology.ru.
##### Нажать на блок "Популярные курсы" в самом низу страницы
##### Нажать на блок "Тестировщик ПО"
##### Откроется страница професии "Тестировщик ПО" https://netology.ru/programs/qa#/
### 2) Переход к форме записи на курс со страницы профессии.
#### **1. Переход к форме записи на курс через "CoursePresentation"**
##### Перейти на страницу профессии, используя один из возможных способов.
##### Нажать кнопку "Записаться" под описанием курса.
##### Откроется форма записи на курс "Тестировщик ПО" https://netology.ru/programs/qa#/order
#### **2. Переход к форме записи на курс через "Header-top"**
##### Перейти на страницу профессии, используя один из возможных способов.
##### Нажать кнопку "Записаться" в вверху страницы.
##### Откроется форма записи на курс "Тестировщик ПО" https://netology.ru/programs/qa#/order
#### **3. Переход к форме записи на курс через скроллинг страницы**
##### Пролистать страницы в самый низ до формы записи на курс https://netology.ru/programs/qa#/order.
### 2) Тестирование формы записи на курс "Тестировщик ПО" - незарегистрированный пользователь
##### 1. HappyPath - имя кириллицей
##### В поле "Имя" ввести имя на русском языке
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту латинскими символами в формате name@.domen
##### Нажать кнопку "Записаться"
##### Проверить то, что в БД появилась данная заявка
##### 2. HappyPath - имя латиницей
##### В поле "Имя" ввести имя на русском языке
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту латинскими символами в формате name@domen.ru
##### Нажать кнопку "Записаться"
##### Проверить то, что в БД появилась запись
##### 3. Invalid - поле "Имя" не заполнено
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту латинскими символами в формате name@.domen.ru
##### Нажать кнопку "Записаться"
##### Под полем "Имя" появляется сообщение об ошибке "Обязательное поле", заявка на обучение не отправляется
##### 4. Invalid - поле "Телефон" не заполнено
##### В поле "Имя" ввести имя
##### В поле "Электронная почта" ввести почту латинскими символами в формате name@.domen.ru
##### Нажать кнопку "Записаться"
##### Под полем "Телефон" появляется сообщение об ошибке "Обязательное поле", заявка на обучение не отправляется
##### 5. Invalid - поле "Электронная почта" не заполнено
##### В поле "Имя" ввести имя
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### Нажать кнопку "Записаться"
##### Под полем "Электронная почта" появляется сообщение об ошибке "Обязательное поле", заявка на обучение не отправляется
##### 6. Invalid - короткое имя
##### В поле "Имя" ввести имя из одной буквы
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту латинскими символами в формате name@domen.ru
##### Нажать кнопку "Записаться"
##### Под полем "Имя" появляется сообщение об ошибке "Должно быть не короче 2 символов", заявка на обучение не отправляется
##### 7. Invalid - некорректный номер телефона
##### В поле "Имя" ввести имя
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99
##### В поле "Электронная почта" ввести почту латинскими символами в формате name@domen.ru
##### Нажать кнопку "Записаться"
##### Под полем "Телефон" появляется сообщение об ошибке "Номер в формате +9 (999) 999-99-99", заявка на обучение не отправляется
##### 8. Invalid - некорректная электронная почта
##### В поле "Имя" ввести имя
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту "testmailru"
##### Нажать кнопку "Записаться"
##### Под полем "Электронная почта" появляется сообщение об ошибке "Неверный email", заявка на обучение не отправляется
##### 9. Invalid - спецсимволы в имени
##### В поле "Имя" ввести имя, используя спецсимволы (.,.+\)
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту "testmailru"
##### Нажать кнопку "Записаться"
##### Под полем "Имя" появляется сообщение об ошибке "Должно состоять из букв", заявка на обучение не отправляется
##### 9. Invalid - иероглифы в имени
##### В поле "Имя" ввести имя, используя иероглифы (入又心凡)
##### В поле "Телефон" ввести номер телефона в формате +7(999)999-99-99
##### В поле "Электронная почта" ввести почту "testmailru"
##### Нажать кнопку "Записаться"
##### Под полем "Имя" появляется сообщение об ошибке "Должно состоять из букв", заявка на обучение не отправляется
## Перечень используемых инструментов с обоснованием выбора
##### Idea
##### Gradle
##### CI
##### Docker
## Перечень необходимых разрешений/данных/доступов
##### Разрешение на проведение тестирования
##### Разрешение на автоматизацию
## Перечень и описание возможных рисков при автоматизации
##### Изменится интерфейс главной страницы или страницы профессии
## Перечень необходимых специалистов для автоматизации
##### Специалист по тестированию
## Интервальная оценка с учётом рисков (в часах)
##### * часов
